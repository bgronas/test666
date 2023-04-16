---
author: "Bengt Grønås"
title: "Automated IaaS Powersaving, Green Sustainability - Pt.1" # Title of the blog post.
date: 2023-03-27T17:43:45+02:00 # Date of post creation.
description: "Contribute to Sustainability by automatically power off and power on of your IaaS workloads as a green service" # Description used for search engine.
featured: false # Sets if post is a featured post, making appear on the home page side bar.
draft: true # Sets whether to render this page. Draft of true will not be rendered.
toc: false # Controls if a table of contents should be generated for first-level links automatically.

# menu: main
usePageBundles: true 

# Set to true to group assets like images in the same folder as this post.
# featureImage: "thumbnail.png" # Sets featured image on blog post.
featureImage: "line.jpg" # Sets featured image on blog post.
# featureImageAlt: 'Description of image' # Alternative text for featured image.
# featureImageCap: 'This is the featured image.' # Caption (optional).

thumbnail: "thumbnail.jpg" # Sets thumbnail image appearing inside card on homepage.
shareImage: "logo.png" # Designate a separate image for social media sharing.
codeMaxLines: 10 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: false # Override global value for showing of line numbers within code block.
figurePositionShow: false # Override global value for showing the figure label.
categories:
  - Technology
tags:
  - Aria
  - Automation
  - Sustainablity
  - green
  - ESG
comment: false # Disable comment if false.
---

**The goal and purpose of this article is to discuss if Powering off VMs in our own infrastructure the same way Google GCP, AWS, and Azure VMs can do on a regular schedule**.** is practical, and show how to do this with VMware technology

## Cloud sustainability and carbon footprint?

You can always argue and debate the various Hyperscaler Cloud computing platforms, such as Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP) about of they already have taken steps towards sustainability and are helping us go green by reducing their carbon footprint, supporting renewable energy development, and developing innovative green technologies. Some of the known statements are:

- AWS (Amazon Web Services). Amazon is committed to being carbon neutral by 2040
- Azure: Microsoft has set a goal to be carbon negative by 2030 and to remove all the carbon it has emitted since its founding in 1975 by 2050
- Google Cloud Platform (GCP): Google is the leader in sustainability initiatives and has been carbon neutral since 2007.
- What about the multi-cloud company VMware?  VMWare did commit to being carbon neutral by 2022, and made it earlier than expected. 

## Hyperscalers and power saving

Hyperscalers use many combinations of power management techniques to optimize energy consumption and reduce their carbon footprint. These techniques can be: 

- If you do not consider mainframe computing, VMware sort of commercialized *Server Consolidation* to reduce energy consumption. This is widely adopted by any hyperscaler, 
- Predictive analytics to anticipate peak usage periods and adjust their power consumption accordingly
- Dynamic power management techniques to adjust the power consumption of their servers based on workload demand.

## Why bother with IaaS?

##### Save money 

Any energy efficiency measures in our datacenter, help us save money by reducing energy consumption and associated costs:

- Reduced Energy Consumption and Bills
- Lower Cooling Costs
- Longer Equipment Lifespan, Reduce the strain on the equipment.
- Improved Resource Utilization. Reduce the need for additional servers
- Reduce operating costs by monitoring VM usage and power consumption, and identify optimization opportunities

##### Promoting sustainability

Companies that support Sustainable Causes and implement Sustainable Practices can meet their sustainability goals. This increases the reputation and the bottom line. Being known as a sustainable through sustainability reports, websites, partnerships and collaborators can attract customers and talent, and create long-term value. The stock market might invest in green organizations, you can get green loans, and the legislation in Europe is becoming more likely to enforce organizations to prove their Green value. 

## Do Hyperscalers power off VMs?

**`Oh yes!`** All the Hyperscalers can schedule VMs to shut down at specific times when they are not needed, such as during off-peak hours or weekends. Some other techniques are Auto-Scaling, load balancing to distribute workloads, idle timeout for VMs. All these techniques helps to reduce energy consumption and optimize resource utilization and reduce their carbon footprint.

### An example on how Google does it

Have a look at Googles “How To” on [Scheduling instances to shut down](https://cloud.google.com/compute/docs/instances/schedule-instance-start-stop#console) . As you can see from this figure it is easy to schedule a shutdown of resources during off-hours.  Here I have created a schedule to Power Off at 18:00:00 and Power On at 06:00:00<img src="./images/index/google_schedule.jpg" style="zoom: 100%;" />



In Part II We will do a technical walk-through using VMware Automation technology



