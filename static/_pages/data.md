---
layout: default
urltitle:  "Data · WAY"
title: "Data · WAY"
permalink: /data
---

<div class="row" style="margin-top:30px;">
  <div class="col-xs-12">
    <h1>Where Are You? Dataset</h1>
  </div>
</div>

<hr>
<div class="row">
  <div class="col-xs-12">
    <p>
      The Where Are You? (WAY) dataset consists of 6,134 human embodied localization dialogs across 87 unique indoor environments. The dataset is constructed on the Matterport3D dataset enviroments using the Matterport3D Simulator and was collected using crowd-sourcing on Amazon Mechanical Turk.
    </p>
  </div>
</div>

<div class="row">
  <div class="col-xs-12">
    <h2>Readme</h2> 
  </div>
  <div class="col-xs-12">
    <p>
      v1.0 contains the processed data that is necessary for the LED task. Additional data is needed to work on the tasks of Embodied Visual Dialog (modeling the Observer) and Cooperative Localization (modeling both agents). Please contact: meerahahn@gatech.edu to get the data and starter code for these tasks. 
    </p>
  </div>



  <div class="col-xs-12">
    <h2>v1.0</h2>
  </div>
  <div class="col-xs-12">
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>train: 4,050 episodes, 58 scenes</li>
      <li>valSeen: 305 episodes, 58 scenes</li>
      <li>valUnseen: 579 episodes, 11 scenes</li>
      <li>test: 1,200 episodes, 18 scenes</li>
   </ul>
  </div>


  <div class="col-xs-12">
    <a
      href="https://drive.google.com/file/d/1gC6Y4jqFOFkKFLSiqkt_ZGU4MM0vYIW7/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'word_embedding', eventValue: 0});"
    >word_embeddings.zip</a> (13 MB)
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Download and place into 'data/language/'</li> 
      <li><code>glove_weights_matrix.npy</code> is extracted from a 300d <a href="https://nlp.stanford.edu/projects/glove/">GloVe</a> file</li>
      <li><code>w2v_weights_matrix.npy</code> is extracted from a 300d <a href="https://github.com/RaRe-Technologies/gensim-data">Word2Vec</a> file</li>
    </ul>
    <br>
    <a
      href="https://drive.google.com/file/d/1_JHaTxty1cnZHnBKUWcNIgAPyCFx0nR7/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'floorplans', eventValue: 0});"
    >floorplans.zip</a> (103 MB)
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Download and place into 'data/floorplans/'</li> 
      <li>Contains top down views of each floor of the house as well as files which associate the pixels on top down maps with Matterport3D panoramic nodes</li>
      <li><code>allScans_Node2pix.json</code> is a dictionary of each scan and its panorama ids. Each panorama id is associated with a list where the first index is the pixel coordinates and the third index is the floor of the house the pano is on. </li>
    </ul>
    <br>
    <a
      href="https://drive.google.com/file/d/1LQ__PGY1KSNjfmGK_YqZezkSwqtdYu9c/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'connectivity', eventValue: 0});"
    >connectivity.zip</a> (2 MB)
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Download and place into 'data/connectivity/'</li> 
      <li>Contains the connectivity of the Matterport3D panoramic nodes</li>
    </ul>
    <br>
    <a
      href="https://drive.google.com/file/d/19env7HjYpgimenS8CJA_1iqoCi_kVDux/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'way_splits', eventValue: 0});"
    >way_splits.zip</a> (2 MB)
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Contains the annotations for the train, val and test splits. In the test split, for each episode we do not provide the finalLocation, navPath or detailedNavPath. Test evaluations should be done on the <a href="https://eval.ai/web/challenges/challenge-page/1206/overview">evaluation and leaderboard server</a>.</li>
      <li>episodeId and socketId is unique to each annotation. </li>
      <li>dialogArray is an array of each message in chronological order alternating between the Locator and the Observer, starting with the Locator. </li>
      <li>navPath is an array of viewpoint ids in chronological order that the Observer visits during the episode.</li>
      <li>detailedNavPath contains the paths taken by the Observer between each round in the dialog. Each array in the list represents a turn of the Observer. Each navigation move is represented by an tuple of [viewpoint, pixel location, floor]. </li>
    </ul>
    <br>
  </div>
  <br>
</div>

<div class="row">
  <br>

  <div class="col-xs-12">
    <h3 style="margin:10px 0;">Format of <code>{split}_data.json</code></h3>
    <pre><code>[
    {
      "episodeId": "3041", 
      "scanName": "5q7pvUzZiYa", 
      "dialogArray": [
                      "what do you see?", 
                      "look for a white couch next to a rug with square patterns that are blue black and white.", 
                      "yup. where are you standing in that room?", 
                      ...
      ],  
      "finalLocation": {
        "viewPoint": "32073c62923f40c590dcac826c72e2a7", 
        "floor": 0, 
        "pixel_coord": [388, 353], 
        "mesh_coord": [1.08773, 0.892166]
      }, 
      "navPath": ["efc16a390eb54273be07a53c9ac005b3", "8c29de2e66404a1faf0d953ae8bb67cf", ...], 
      "detailedNavPath": [
        ["efc16a390eb54273be07a53c9ac005b3", ..., "32073c62923f40c590dcac826c72e2a7"], 
        ["32073c62923f40c590dcac826c72e2a7", ..., "32073c62923f40c590dcac826c72e2a7"]
      ], 
      "socketId": "xVc8PpN1yMkdtRafAATMxYipgp5ZDsWP8McmAATL"
    },
    ...
    ]</code></pre>
  </div>
</div>

<div class="row">
  <div class="col-xs-12">
    <h2>Trained Models to download for LED Task</h2> 
  </div>
  <div class="col-xs-12">
    <a
      href="https://drive.google.com/file/d/1WTHyDEpn-4wRnvGkXCm_g7bm5_gBB8oQ/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'base', eventValue: 0});"
    >lingunet-skip.pt</a> (65.7 MB)
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Download and place into 'data/models/lingunet-skip.pt'</li> 
      <li>Contains the trained lingunet-skip model described in the paper for the LED task.</li>
    </ul>
    <br>
    <a
      href="https://drive.google.com/file/d/1kvUofiaMCz6g6f1BWfvSnO32aU278HUi/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'base', eventValue: 0});"
    >crossmodal_simple.pt</a> (72.2 MB)
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Download and place into 'data/models/crossmodal_simple.pt'</li> 
      <li>Contains the trained simple crossmodal model to predict the best viewpoint on the navigation graph.</li>
    </ul>
    <br>
    <a
      href="https://drive.google.com/file/d/1qB-r1sybtJNH3siIoGQ4J3CToyc4BRTK/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'base', eventValue: 0});"
    >crossmodal_att.pt</a> (67.4 MB)
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Download and place into 'data/models/crossmodal_att.pt'</li> 
      <li>Contains the trained crossmodal model with attention to predict the best viewpoint on the navigation graph.</li>
    </ul>
  </div>
