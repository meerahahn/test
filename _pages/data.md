---
layout: default
urltitle:  "Data · NRNS"
title: "Data · NRNS"
permalink: /data
---

<div class="row" style="margin-top:30px;">
  <div class="col-xs-12">
    <h1>Image-Goal Navigation Splits</h1>
  </div>
</div>

<hr>



<div class="row">
  <div id=content class="col-xs-12">
    <img src="static/img/nrns/image_goal_nav.jpg" alt="">
    <p>
      We provide test splits for the Image-Goal navigation task for Matterport3D and Gibson datasets. We provide multiple splits for each dataset which are divded based on difficulty. Specifically sub-divide test episodes into two categories: `straight' and `curved'. In `straight' episodes the ratio of shortest path geodesic-distance to euclidean-distance between the start and goal locations is < 1.2 and rotational difference between the orientation of the start position and goal image is < 45 degrees. All other start-goal location pairs are labeled as `curved' episodes. We make this distinction to test narrow field of view agents. We further subdivide each of these 2 categories into 3 difficulty sub-categories: `easy', `medium' and `hard'. Difficulty is determined by length of the shortest path between the start and goal locations. The `easy', `medium' and `hard' settings are (1.5-3m), (3-5m), and (5-10m) respectively. We generated these test episodes by uniformly sample start-goal location pairs from the test scenes to create approximately 1000 episodes per setting.  
    </p>
  </div>
</div>


<div class="row">
  <div class="col-xs-12">
    <h2>Matterport splits</h2>
  </div>
  <div class="col-xs-12">
    <a
      href="https://drive.google.com/file/d/1J7Qvc0yILSmGDLyzSJmYjJ5TFx1UWR8f/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'word_embedding', eventValue: 0});"
    >matterport_test_splits.zip</a> (1 MB)
  </div>
  <div class="col-xs-12">
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Straight- Easy: 1,000 episodes, 18 scenes</li>
      <li>Straight- Medium: 1,000 episodes, 18 scenes</li>
      <li>Straight- Hard: 1,000 episodes, 18 scenes</li>
      <li>Curved- Easy: 1,000 episodes, 18 scenes</li>
      <li>Curved- Medium: 1,000 episodes, 18 scenes</li>
      <li>Curved- Hard: 1,000 episodes, 18 scenes</li>
   </ul>
  </div>
  <div class="col-xs-12">
    <h2>Gibson splits</h2>
  </div>
  <div class="col-xs-12">
    <a href="https://drive.google.com/file/d/1TCv2cOEqNRKI3bQbsvNbLS63_qKy8h_l/view?usp=sharing"
      onClick="ga('send', 'event', { eventCategory: 'download', eventAction: 'click', eventLabel: 'word_embedding', eventValue: 0});"
    >gibson_test_splits.zip</a> (1 MB)
  </div>
  <div class="col-xs-12">
    <ul style="margin:10px 10px 10px;"  class="col-xs-12">
      <li>Straight- Easy: 1,000 episodes, 14 scenes</li>
      <li>Straight- Medium: 1,000 episodes, 14 scenes</li>
      <li>Straight- Hard: 806 episodes, 14 scenes</li>
      <li>Curved- Easy: 1,000 episodes, 14 scenes</li>
      <li>Curved- Medium: 1,000 episodes, 14 scenes</li>
      <li>Curved- Hard: 1,000 episodes, 14 scenes</li>
   </ul>
  </div>
</div>
