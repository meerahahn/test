---
layout: default
urltitle:  "WAY-LED"
title: "Where Are You? Localization via Embodied Dialog"
categories: deep learning, computer vision, natural language processing, machine learning
permalink: /
favicon: /static/img/way/favicon2.png
---

<br>

# Dataset: Where Are You? (WAY) {#overview}

<div class="row">

  <div class="col-xs-12 text-center">
    <br>
    <img src="{{site.baseurl}}/static/img/way/WAY.jpg" alt="WAY dataset">
  </div>

  <div class="col-xs-12">
    <br>
    <p>
      The Where Are You? (WAY) dataset contains ~6k dialogs in which two humans -- an Observer and a Locator -- complete a cooperative localization task. The Observer is spawned at random in a 3D environment and can navigate from first-person views while answering questions from the Locator. The Locator must localize the Observer in a map by asking questions and giving instructions. Based on this dataset, we define three challenging tasks: Localization from Embodied Dialog or LED (localizing the Observer from dialog history), Embodied Visual Dialog (modeling the Observer), and Cooperative Localization (modeling both agents).
    </p>
    <br>
  </div>
</div>

# Task: Localization via Embodided Dialog (LED) {#overview}

<div class="row">

  <div class="col-xs-12">
    <br>
    <p>
      Localization from Embodied Dialog (LED), is the state estimation problem of localizing the Observer given a map and a partial or complete dialog between the Locator and the Observer. This task specifically tests a models ability to accurately encode a dialog and effectively ground it into the visual representation of an environment.
    </p>
    <br>
  </div>

  <div class="col-xs-12 text-center">
      <br>
    <img src="{{site.baseurl}}/static/img/way/LED.jpg" alt="LED Task">
  </div>

  <div class="col-xs-12 text-center">
    <br>
    <h3>
    <b>
    The WAY codebase and most recent LED models are available at:<br><a class="poplink" href="https://github.com/meera1hahn/Graph_LED/">https://github.com/meera1hahn/Graph_LED/</a>
    </b>
    </h3>
    <br>
    <h3>
    <b>
    The test server and leaderboard is live on EvalAI:<br><a class="poplink" href="https://eval.ai/web/challenges/challenge-page/1206">https://eval.ai/web/challenges/challenge-page/1206</a>
    </b>
    </h3>
  </div>
</div>
<hr>

# News {#news}

<div class="row">
  <div class="col-xs-12">
    <span style="color:#e74c3c;font-weight:400;">July 2021</span> — The public leaderboard is now <a href="https://eval.ai/web/challenges/challenge-page/1206/overview">live on EvalAI</a>!
  </div>
  <div class="col-xs-12">
    <span style="color:#e74c3c;font-weight:400;">July 2021</span> — <a href="https://github.com/meera1hahn/Graph_LED/">PyTorch code and models for the LED task is based on the navigation graph is now available</a>! Contains multiple models including cross modal embeddings and lingunet-skip. 
  </div>
  <div class="col-xs-12">
    <span style="color:#e74c3c;font-weight:400;">January 2021</span> — <a href="https://github.com/batra-mlp-lab/WAY/">PyTorch code for the lingunet model and ablations in the paper is now available</a>!
  </div>
  <div class="col-xs-12">
    <span style="color:#e74c3c;font-weight:400;">November 2020</span> — Paper accepted to <b>EMNLP 2020</b>!
  </div>
  <div class="col-xs-12">
    <span style="color:#e74c3c;font-weight:400;">November 2020</span> — <a href="https://meerahahn.github.io/way/data">WAY dataset</a> is now available!
  </div>
  </div>
<hr>

# Paper {#paper}


<div class="row">
    <div class="col-xs-12">
        <h3>Where Are You? Localization from Embodied Dialog</h3>
    </div>
    <div class="col-xs-12" style="margin-top: 3px; color: #666;">
        Meera Hahn, Jacob Krantz, Dhruv Batra, Devi Parikh, James M. Rehg, Stefan Lee, Peter Anderson<br>
    </div>
    <div class="col-xs-12" style="margin-top: 3px; color: #666;">
      ECCV 2020
      [<a href="{{site.baseurl}}/bib/way.bib.txt">Bibtex</a>]
      [<a href="https://arxiv.org/pdf/2011.08277.pdf">PDF</a>]
      [<a href="https://github.com/meera1hahn/Graph_LED/">Code</a>]
    </div>
</div>
<div class="row">
    <div class="col-xs-12">
        <a href="https://arxiv.org/pdf/2011.08277.pdf">
          <img class="thumb" src="{{site.baseurl}}/static/img/way/thumb.jpg">
        </a>
    </div>
</div>

<div class="row">
  <div class="col-xs-12">
    <img src="{{site.baseurl}}/static/img/way/lingunet.jpg">
  </div>
</div>
<br>

<div class="row">
  <div class="col-xs-12">
    <div class="vid-container">
      <iframe src="https://www.youtube.com/embed/RtIq_YXpiXY" allowfullscreen></iframe>
    </div>
  </div>
</div>
<br>
<hr>

# People {#people}

<br>
<div class="row">
  <div class="col-md-2 col-md-offset-2 col-sm-3 col-xs-6">
    <a href="https://meerahahn.github.io/">
      <img class="people-pic" src="/way/static/img/people/meera.jpg" />
    </a>
    <div class="people-name">
      <a href="https://meerahahn.github.io/">Meera Hahn</a><br />
      <affiliation>Georgia Tech</affiliation>
    </div>
  </div>
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="https://jacobkrantz.github.io/">
      <img class="people-pic" src="/way/static/img/people/jacob.jpg" />
    </a>
    <div class="people-name">
      <a href="https://jacobkrantz.github.io/">Jacob Krantz</a><br />
      <affiliation>Oregon State University</affiliation>
    </div>
  </div>
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="https://www.cc.gatech.edu/~dbatra/">
      <img class="people-pic" src="/way/static/img/people/dhruv.jpg" />
    </a>
    <div class="people-name">
      <a href="https://www.cc.gatech.edu/~dbatra/">Dhruv Batra</a><br />
      <affiliation>Georgia Tech &amp; Facebook AI Research</affiliation>
    </div>
  </div>
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="https://www.cc.gatech.edu/~parikh/">
      <img class="people-pic" src="/way/static/img/people/devi.jpg" />
    </a>
    <div class="people-name">
      <a href="https://www.cc.gatech.edu/~parikh/">Devi Parikh</a><br />
      <affiliation>Georgia Tech &amp; Facebook AI Research</affiliation>
    </div>
  </div>  
</div>
<div class="row">
  <div class="col-md-2 col-md-offset-3 col-sm-3 col-xs-6">
    <a href="http://www.cc.gatech.edu/~rehg/">
      <img class="people-pic" src="/way/static/img/people/jim.jpg" />
    </a>
    <div class="people-name">
      <a href="http://www.cc.gatech.edu/~rehg/">James M. Rehg</a><br />
      <affiliation>Georgia Tech</affiliation>
    </div>
  </div>   
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="http://web.engr.oregonstate.edu/~leestef/" style="border:0;">
      <img class="people-pic" src="/way/static/img/people/stefan.jpg" />
    </a>
    <div class="people-name">
      <a href="http://web.engr.oregonstate.edu/~leestef/">Stefan Lee</a><br />
      <affiliation>Oregon State University</affiliation>
    </div>
  </div>  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="https://panderson.me/" style="border:0;">
      <img class="people-pic" src="/way/static/img/people/peter.jpg" />
    </a>
    <div class="people-name">
      <a href="https://panderson.me/">Peter Anderson</a><br />
      <affiliation>Google</affiliation>
    </div>
  </div>
</div>
<hr>

<!-- # Acknowledgements -->

<!-- <a name="{{site.baseurl}}/acknowledgements"></a>
<div class="row">
  <div class="col-xs-12">
    <p>
      Add acknowledgements here 
    </p>
  </div>
</div>
<hr> -->

<div class="row">
  <div class="col-xs-6">
    <span style="font-weight:400;">Email</span> — meerahahn@gatech.edu
  </div>
  <br>
</div>