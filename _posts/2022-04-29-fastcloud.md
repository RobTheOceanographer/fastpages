---
keywords: fastai
description: A small project to start my fastai journey.
title: FastClouds - my first fastai model
comments: true
categories: [fastai, jupyter, clouds, meteorology]
image: images/cloud_batch_small.png
nb_path: _notebooks/2022-04-29-fastcloud.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-04-29-fastcloud.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>I am currently a student in the <a href="https://course.fast.ai/">fast.ai practical deep learnign for coders v5</a> class and after the first week I took <a href="https://twitter.com/jeremyphoward">Jeremy's</a> advice to just try to complete some small project using the material covered so far in lesson 1.</p>
<p>Therefore, I humbly present <strong><em>FastClouds</em></strong></p>
<p>This is not meant to be a serious project and is just for my own learning experience.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="The-Problem">The Problem<a class="anchor-link" href="#The-Problem"> </a></h2><p>On ground observations are a key part to weather forecasting. Most observations are taken by autonomous systems but there are still a few routine observations that are done manually by a human. One of these is cloud type classification.</p>
<p>This manual observation is currently done is at major airports around Australia. At these airports one or more highly knowledgeable and accredited aerodrome weather observers is stationed to take manual weather observations on a fixed schedule throughout each day. But, having such specialized observers at all airports all of the time is not cost effective or realistically feasible, especially for remote locations (e.g. uninhabited islands or infrequently used aerodromes). Therefore many of these remote or small areas miss out on observations and perhaps receive lower quality situational awareness and forecasts as a result.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="The-Solution">The Solution<a class="anchor-link" href="#The-Solution"> </a></h2><p>Using deep learning and image classification techniques to classifying cloud types from photographs seemed to me a very plausible solution to this problem. Therefore, after the Fastai course v5 lecture 1 I thought I'd try to do exactly that using a visual learner example Jeremy provided as my starting point.</p>
<p>This algorithm uses a resnet and transfer learning as per the original notebook - [is-it-a-bird] -(<a href="https://www.kaggle.com/code/jhoward/is-it-a-bird-creating-a-model-from-your-own-data">https://www.kaggle.com/code/jhoward/is-it-a-bird-creating-a-model-from-your-own-data</a>) but it uses three broad categories of clouds instead of just birds vs forests. These classes were chosen as per the work of Luke Howard in "Essay of the Modifications of Clouds" (1803).</p>
<p><img src="images/copied_from_nb/images/cloud_types.png" alt="">
<img src="images/copied_from_nb/my_icons/fastai_logo.png" alt="">
This is an image from: <a href="https://www.weather.gov/jetstream/corefour">https://www.weather.gov/jetstream/corefour</a></p>
<p>In order to create a data set duckduckgo was searched for the terms: cirrus clouds, cumulus clouds, stratus clouds. here is an example batch of images used in the training:</p>
<p><img src="images/copied_from_nb/images/cloud_batch_big.png" alt=""></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="The-Notebook">The Notebook<a class="anchor-link" href="#The-Notebook"> </a></h2><p>This notebook is sitting on <a href="https://www.kaggle.com/">Kaggle</a> as it has a nice (e.g. free...) gpu backend that allows you to run this model should you wish to poke around.</p>
<p><strong><em>So, here it is for you to enjoy - <a href="https://www.kaggle.com/robtheoceanographer/fastclouds">https://www.kaggle.com/robtheoceanographer/fastclouds</a></em></strong></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Conclusion">Conclusion<a class="anchor-link" href="#Conclusion"> </a></h2><p>While this is very basic demo and only about 70% accurate, it shows great potential for automating some of the cloud type observing in remote regions of Australia where there is currnetly limited or no human observer coverage, and therefore this work might benifit from future work.</p>
<p>I'd love ideas, feedback, and suggestions should anyone have any.</p>
<p>Thanks</p>

</div>
</div>
</div>
</div>
 
