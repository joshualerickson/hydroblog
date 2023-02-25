---
title: gsutil workflow
author: Josh Erickson
date: '2021-03-04'
slug: []
categories: []
tags: []
description: ''
---
# Working with gsutil

## Introduction

This is a workflow on how to download multiple objects from a bucket on google cloud storage. Basically, so I stop forgetting how to do it.

#### Moving objects

Technically, you can create your own folders via some (above my head) method but I'll just default to using the UI on GCS. From there, you can then start to move files that you've uploaded via desktop, R, earth engine, etc. To do that use the code below in the `Google Cloud SDK Shell`

    gsutil mv gs://your-bucket/some_file.tif gs://your-bucket/some-other-folder

So, now that you have objects where you want them to be you can then start downloading. You could technically move `mv` objects to the desktop **but** they will then not be on the cloud anymore 😞.

#### Downloading

There are a couple ways to get objects from your GCS to your desktop via download: download one-by-one, download with wildcard \*, or download in parallel. We'll go through one-by-one and parallel.

one-by-one;

    gsutil cp gs://your-bucket/some_file.tif D:/some-directory

parallel;

    gsutil -m cp -r gs://jle_rasters/*.tif D:/R_folder/Rasters/cbi/R1_test/

And that's it! There's way way more you can do but this is really the majority of my workflow so we'll stop here.
