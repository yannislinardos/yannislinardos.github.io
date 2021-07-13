---
layout: description
title: My Projects
permalink: /projects/
---    

## [Signal Quality Assessment for Reliable Fetal Heart Rate Detection Using Deep Learning](https://github.com/yannislinardos/fetalHeartrateDetection)

<div style="text-align: justify">

The present work is concerned with assessing the signal quality of a four-channel non-invasive fetal ECG recording. The fetal ECG recordings contain multiple fetal and maternal noise sources and are destined to be used to estimate the Fetal Heart Rate (FHR). High signal quality is associated with reliable FHR estimation and low quality with unreliable. We approached the topic from the perspective of anomaly detection, in which low quality signals are considered anomalies. For this purpose, two deep learning-based approaches for anomaly detection were explored. The first approach consisted of autoencoders trained on data considered non-anomalous. Then, the reconstruction error serves as an anomaly metric. To encapsulate the temporal interdependence of the data, we used an LSTM classifier that labelled a segment as an anomaly based on its reconstruction error as well as the reconstruction errors of the segments that preceded it. Two autoencoders were developed, one operating on the time domain and one on the frequency domain. The resulting final pipeline has relatively adequate performance. The second approach was the GAN based anomaly detection. In this technique, a GAN is trained to generate data that are considered non-anomalous using a random vector input sampled from a latent space. Afterwards, a query sample is mapped to this latent space, something that can be done with a few techniques that we discuss, and the mapped latent vector is used to re-generate the segment. The fidelity of the re-generated sample serves as an anomaly score. GAN-based anomaly detection can be conducted locally; so we can train GANs to generate long signals and assess the quality in their segments. In order to generate signals, we proposed a new GAN architecture aimed to generate signals based on their frequency representation. Unfortunately, the GAN based anomaly detection did not work on the target dataset. However, it did work successfully on a simpler dataset, showcasing its efficacy.
   </div>

##  [Multiscale Convolutions for an Artificial Neural Network](https://github.com/yannislinardos/Multiscale-CNN)

  <div style="text-align: justify">
    
The study investigates the possibility of using convolutional neural networks across input of different sampling rates, focusing on one-dimensional convolutions. This is an idea that has not been adequately studied although it may produce useful results that expand the usefulness of convolutional neural networks. The problem was approached from the perspective of algebraic multigrid. Three interpolation methods were tested on audio classification neural networks trained for input of different sampling rates: nearest neighbor, linear interpolation and inverse distance weighting. The approach was extended to pooling and fully connected layers. In the case of using a neural network trained for high sampling rate input with input of low resolution, the method of linear interpolation gave promising results. Moreover, the results hint that pooling layers should not be changed in the process of multiscaling. In the case of training for low sampling rate and testing with input of high sampling rate, there is no unique solution to the system of weight equations. In dealing with this problem, the approach of directly prolonging the convolution kernels was tried using the three interpolation methods that were explained above as well as the method of kernel dilation. The last method, kernel dilation, appeared to be considerably effective in upscaling.
   </div>

## [Annotation Tool for NLP](https://github.com/yannislinardos/annotationTool)
  
  <div style="text-align: justify">

The radiologists of MRON in collaboration with ZGT (ZiekenhuisGroep Twente / Hospital Group Twente) are doing research on innovations in radiology using AI. For a large part, this research focuses on Natural Language Processing technology, because whenever radiologists evaluate an X-Ray/CT/MRI/etc, they write a textual report. Although they call it a "structured report", it is plain text, unstructured data from a computer science perspective. The "structured" refers to the fact that it complies with the international BI-RADS standard. Their goal is to use Natural Language Processing in order to extract actual structured data (i.e. in XML or json format) from a “structured” natural language report.

However, one of the main problems in Natural Language processing is how to obtain properly annotated data to train the classifiers. This usually happens manually; a very monotonous and intensive work.

The goal of this project is to design and develop an annotation tool that will facilitate this process by making the manual annotation as efficient as possible. This means building a user friendly application that runs smoothly and can be integrated to the hospital work-flow. Moreover, we integrate a Natural Language Processing classifier that is trained to automatically annotate radiology reports with the BIRADS standard. These automatically annotated reports can be checked and accepted or rejected by a human annotator in a later phase. This will make the annotation work semi-automatic.

Although the main target group is radiologists writing reports in the BIRADS standard, we allow for different annotation systems to be defined so that the application usage can be extended to other departments of the hospital.
       </div>

## [Style Transfer via CycleGAN](https://github.com/yannislinardos/cycleGAN)
   <div style="text-align: justify">   

In machine learning, the study of generative adversarial networks (GANs) is currently one of the most exciting topics. In brief, in GANs, the generator and thediscriminator compete in a game with each other with the goal of generating new data that can pass for real data.In this project, we will explore two types of GANs - Deep Convolutional GAN (DCGAN) and CycleGAN, with more emphasis on the latter. DCGAN is used to generate emojis and CycleGAN is used to transform the style of one image to another. The results show that the cycle consistency losshas improved the results of the CycleGAN model. In the case of DCGAN, mode collapse was observed.
   </div>

## [Twitter Reaction on the Moscow Protests 2019](https://github.com/yannislinardos/twitterMoscowProtests)
   <div style="text-align: justify">   

Twitter is a widely used online platform for stating opinions and sharinginformation with other people. This is a research on the manner Russian users communicated through Twitter during the protests occurring in Moscow in July and August 2019. Both quantitative and qualitative analysis was conducted; twitter data was analyzed in regards to their amount in different metrics (users, hashtags, number of tweets) as well as the expressed emotions and opinions. Twitter data was compared with what happened on the streets in regards to attendance.

In order to evaluate reactions on Twitter, data was taken from archive.org, a non-profit internet archive of resources, like books, videos and websites. Twitter data was downloaded for a period of 43 days (19th of July until the 31st of August 2019) from the provided archive; this includes about 2% of all actual global Twitter data as given by the Twitter API. This resulted in about 250 Gb of raw data or 83.3 Gb of compressed data. For conducting this work, Python 2.7 was used with the modules PySpark (mainly the SQL module) for data preprocessing and processing as well as NumPy and Matplotlib for evaluating and representing the results. Moreover, we used the Python modules NLTK and pymorphy2 to perform the sentimentanalysis.
     </div>

## [Satelite Capacity Allocation using Markov Decision Process](https://github.com/yannislinardos/satelite_capacity_mdp)

  <div style="text-align: justify">
      
The problem is the optimization of a satellite network controller where messages from two sources arrive. This problem can be handled as a queuing system with two independent Poisson arrival processes. The satellite network controller has no queue and has a limited capacity, therefore the messages that the controller does not admit will never be handled. With this rejection, some costs arise. Messages that are admitted will be handled for some discrete time units. The number of time units they will be handled for has a certain probability distribution. The purpose is to create a policy for the controller of the satellite network in regards to which messages it has to admit and which messages it has to reject in order to minimize the costs.
    
   </div>
## [Nomadic Tracker Problem using Approximate Dynamic Programming](https://github.com/yannislinardos/nomadic_tracker_mdp)
        
  <div style="text-align: justify">

Assume a truck may move to 20 cities, loaded or unloaded. The truck receives a reward when it visits a city on which there is demand, otherwise it incurs a cost. Demand is random. This project is about calculating the optimal policy of the truck using approximate dynamic programming.

  
   </div>
