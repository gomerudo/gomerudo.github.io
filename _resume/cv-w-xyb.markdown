---
layout: milestone
title: XYB
description: DevOps Engineer (Remote)
date-start: 2017-09-01
date-end: 2018-08-31
img: /img/xyb.png
---

As a side activity that allowed me to afford my living expenses during my time as a master student, I collaborated as a DevOps engineer with <a href="https://www.linkedin.com/company/xyb/" target="_blank">XYB</a>, a small-size software company in Los Angeles. The collaboration started as a basic Continous Integration setup and escalated to a more complex AWS architecture.

It is possible to explain the work in two stages. In the first stage, I set up and configured a Jenkins server, on an EC2 instance, to build and deploy *development* and *production* pipelines. This part included integration with third-party services such as GitHub and Slack, different Linux management operations, and NGINX maintenance.

In the second stage, the architecture became ECS-based using Docker containers. Different services (including Jenkins) were dockerized and deployed via Go scripting to ECS, S3, and CloudFront.
