---
layout: default
urltitle:  "NRNS"
title: "No RL, No Simulation: Learning to Navigate without Navigating"
categories: deep learning, computer vision, machine learning, robotics, navigation
permalink: /
favicon: /static/img/nrns/favicon2.png
---

<br>

# NRNS: No RL, No Simulation {#overview}

<div class="row">

  <div class="col-xs-12 text-center">
      <video width="960" height="360" autoplay="autoplay" controls="controls" muted>
        <source src="{{site.baseurl}}/static/img/nrns/teaser.mp4" type="video/mp4">
      </video>
  </div>

  <div class="col-xs-12 text-center">
    <p>
      We pose a simple question: Do we really need active interaction, ground-truth maps or even reinforcement-learning (RL) in order to solve the image-goal navigation task? We propose a self-supervised approach to learn to navigate from only passive videos of roaming and demonstrate the success of this approach on Image-Goal navigation in unseen environments. The No RL, No Simulator (NRNS) is a hierarchical modular approach that builds and maintains a topological map. Using a passively trained distance function and target direction prediction function the agent selects and navigates to sub-goals before terminating at the predicted goal location. We gather passive videos from random walks in simulators and YouTube and use these videos to train the NRNS modules. 
    </p>
    <img src="{{site.baseurl}}/static/img/nrns/teaser.jpg" alt="NRNS module">
  </div>
</div>
<hr>

# Task: Image-Goal Navigation {#overview}

<div class="row">

  <div class="col-xs-12">
    <br>
    <p>
      We tackle the task of image-goal navigation, where an agent is placed in a novel environment, and is tasked with navigating to an (unknown) goal position that is specified using an image taken from that position. More formally, an episode begins with an agent receiving an RGB observation corresponding to the goal position. At each time step, of the episode the agent receives a set of observations, and must take a navigation action. The agents state observations, are defined as a narrow field of view RGBD, and egocentric pose estimate. The agent must use a policy to navigate to the goal before reaching a maximum number of actions. 
    </p>
    <br>
  </div>
<!-- 
  <div class="col-xs-12 text-center">
      <br>
    <img src="{{site.baseurl}}/static/img/nrns/nrns.jpg" alt="LED Task">
  </div> -->

  <!-- <div class="col-xs-12 text-center">
    <br>
    <h3>
    <b>
    The NRNS codebase and models are available at:<br><a class="poplink" href="https://github.com/meera1hahn/NRNS/">github.com/meera1hahn/NRNS/</a>
    </b>
    </h3>
  </div> -->
</div>
<hr>

# News

<div class="row">
  <div class="col-xs-12">
    <span style="color:#e74c3c;font-weight:400;">October 2021</span> — Arxiv version and PyTorch code for training and evaluating agent on image-goal are out!<br>
    <span style="color:#e74c3c;font-weight:400;">September 2021</span> — Accepted to NeurIPS!
  </div>
</div>
<hr>

# Paper

<div class="row">
    <div class="col-xs-12">
        <h3>No RL, No Simulation: Learning to Navigate without Navigating</h3>
    </div>
    <div class="col-xs-12" style="margin-top: 3px; color: #666;">
        Meera Hahn, Devendra Chaplot, Shubham Tulsiani, Mustafa Mukadam, James M. Rehg, Abhinav Gupta<br>
    </div>
    <div class="col-xs-12" style="margin-top: 3px; color: #666;">
      2021
      [<a href="{{site.baseurl}}/bib/nrns.bib.txt">Bibtex</a>]
      [<a href="https://arxiv.org/abs/2110.09470">PDF</a>]
      [<a href="https://github.com//meera1hahn/NRNS">Code</a>]
    </div>
</div>
<div class="row">
    <div class="col-xs-12">
        <a href="https://arxiv.org/abs/2110.09470">
          <img class="thumb" src="{{site.baseurl}}/static/img/nrns/thumb.jpg">
        </a>
    </div>
</div>
<br>
<hr>


<div class="row">
  <div class="col-xs-12">
    <div class="vid-container">
      <iframe src="https://www.youtube.com/embed/6YxmkjtJomA" allowfullscreen></iframe>
    </div>
  </div>
</div>
<br>
<hr>


# People

<br>
<div class="row">
  <div class="col-md-2 col-md-offset-2 col-sm-3 col-xs-6">
    <a href="https://meerahahn.github.io/">
      <img class="people-pic" src="/nrns/static/img/people/meera.jpg" />
    </a>
    <div class="people-name">
      <a href="https://meerahahn.github.io/">Meera Hahn</a><br />
      <affiliation>Georgia Tech</affiliation>
    </div>
  </div>
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="https://devendrachaplot.github.io/">
      <img class="people-pic" src="/nrns/static/img/people/devendra.jpg" />
    </a>
    <div class="people-name">
      <a href="https://devendrachaplot.github.io/">Devendra Chaplot</a><br />
      <affiliation>Carnegie Mellon &amp; Facebook AI Research</affiliation>
    </div>
  </div>
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="http://www.mustafamukadam.com/">
      <img class="people-pic" src="/nrns/static/img/people/mustafa.jpg" />
    </a>
    <div class="people-name">
      <a href="http://www.mustafamukadam.com/">Mustafa Mukadam</a><br />
      <affiliation>Facebook AI Research</affiliation>
    </div>
  </div>
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="http://www.cc.gatech.edu/~rehg/">
      <img class="people-pic" src="/nrns/static/img/people/jim.jpg" />
    </a>
    <div class="people-name">
      <a href="http://www.cc.gatech.edu/~rehg/">James M. Rehg</a><br />
      <affiliation>Georgia Tech</affiliation>
    </div>
  </div>   
</div>
<div class="row">
  <div class="col-md-2 col-md-offset-4 col-sm-4 col-xs-6">
    <a href="http://shubhtuls.github.io/">
      <img class="people-pic" src="/nrns/static/img/people/shubham.jpg" />
    </a>
    <div class="people-name">
      <a href="http://shubhtuls.github.io/">Shubham Tulsiani</a><br />
      <affiliation>Facebook AI Research</affiliation>
    </div>
  </div>  
  <div class="col-md-2 col-sm-3 col-xs-6">
    <a href="http://www.cs.cmu.edu/~abhinavg/" style="border:0;">
      <img class="people-pic" src="/nrns/static/img/people/abhinav.jpg" />
    </a>
    <div class="people-name">
      <a href="http://www.cs.cmu.edu/~abhinavg/">Abhinav Gupta</a><br />
      <affiliation>Carnegie Mellon &amp; Facebook AI Research</affiliation>
    </div>
  </div>
</div>
<hr>
<div class="row">
  <div class="col-xs-6">
    <span style="font-weight:400;">Email</span> — meerahahn@gatech.edu
  </div>
  <br>
</div>