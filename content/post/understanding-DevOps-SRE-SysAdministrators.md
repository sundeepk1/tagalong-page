---
title: "Understanding DevOps SRE SysAdministrators"
date: 2020-10-16T12:17:20+08:00
toc: true
tags: 
  - "DevOps"
  - "SRE"
  - "System Administration"
draft: false
sidebar: "right"
---

Let’s start with the first part of our journey, And that's understanding what is DevOps,SRE, How is it different from the traditional roles that we know - “Linux Administration”. What do they do and what makes them so important for an organization? How can you become a SRE/DevOps Engineer? 

## What is DevOps?
DevOps has different connotations to different people. The most common understanding is that it is a portmanteau of “Development” and “Operations”, hence DevOps. For evangelists, DevOps is a culture and a transformation. For some engineers, DevOps is a set of agile tools and techniques. For managers, DevOps is probably a methodology. For other people it is just a buzzword and for recruiters, DevOps is a job role. Every organization has their own understanding and culture around DevOps.

To start with, we have to understand that DevOps is not all about Tools, Automation or a team or a person who does DevOps or about the developer who is developing the software product. Let’s deconstruct DevOps. In order to understand DevOps, it's principles and values delivered, we need to have a general idea about Software development lifecycle (SDLC). 

Traditionally, Software is developed by developers and then handed over to the Operations team for deploying it to the production environment. There are some well known software methodology for developing software - Waterfall and Agile. For now, understand that the waterfall model is a time consuming methodology whereas Agile is a faster way of developing software and has become very popular in the recent decades.I will have a post later on this topic - “Software development methodology”. 

DevOps team works closely with the Development team and plays a vital role in the Software development lifecycle (SDLC). What is SDLC, it’s a sequence of steps followed to develop a software product or feature. Primarily, it consists of 

1. Requirements Gathering 
2. Planning
3. Design
4. Development 
5. Testing 
6. Deployment

Long story short, Devops is a way of work (Philosophy) and not the work itself. The value from DevOps philosophy can be achieved when the Developers and the operations team break the silos and work hand in hand.  

Please refer to the resources below for more reading and to create an in-depth understanding of DevOps. 

Quite often, DevOps is directly associated with Automation, Continuous Integration, Continuous Delivery etc. which is a way of getting value from DevOps adoption. One of the frameworks that can be associated is CALMS. 

* Culture - people and process
* Automation - Automate repeated tasks 
* Lean - Applying Lean principles to IT
* Metrics - Measure extensively and use to improve 
* Sharing - Continuous learning by sharing knowledge 

The correlation of DevOps with SDLC can be depicted as below.

![How DevOps LifeCycle is related to SDLC](/img/DevOps-Intro/devops-SDLC.png)

### What makes a great DevOps Engineer?
Today DevOps, is one of the major key terms for job search and it has become a hot job role. In my opinion the job role is very demanding and one must be prepared for a continuous learning and upskilling path. We can categorize and list the below few skills that are sought after by most of the employers. 

| Category                                  | Tools/Softwares                                                |
|-------------------------------------------|----------------------------------------------------------------|
| Operating Systems                         | Linux (CentOS/RedHat)                                          |
| Infrastructure as a code                  | Terraform                                                      |
| Cloud Platforms                           | Google Cloud Platform, Amazon Web Services, Microsoft Azure    |
| Configuration Management Tools            | Ansible, Chef, Puppet                                          |
| Source Code Management Tools              | Git, Github, BitBucket                                         |
| Continuous Integration/Deployment Tools   | Jenkins, Concourse, CircleCI                                   |
| Containerization and Orchestration        | Docker, Kubernetes                                             |
| Programming/ Scripting                    | Bash, Python                                                   |
| Build Tools & Repository Management       | Maven, Gradle, JFrog Artifactory                               |
| Code Quality                              | SonarQube                                                      |
| Database Administration                   | MySQL, MongoDB, Redis                                          |
| Message Queuing/ Streaming                | Apache Kafka, RabbitMQ                                         |
| Middlewares                               | Apache httpd, Nginx, Apache TomCat                             |
| Logging and Monitoring                    | Elasticsearch, Prometheus                                      | 
| Collaboration Tools                       | JIRA, Confluence                                               |

Certainly the above list of tools looks intimidating and overwhelming, however with practice and time you would have an appreciation for each of these tools and would learn them. 


### How can I become one?

As we can see from the list of skills expected from employers, one has to learn the tools and practice them on a daily basis in order to get the hang of the tools and that would in turn help one to navigate the waters. 

### Resources

#### Books
[The DevOps Handbook: How to Create World-Class Agility, Reliability, and Security in Technology Organizations, by Gene Kim , Patrick Debois , et al.](https://www.amazon.com/DevOps-Handbook-World-Class-Reliability-Organizations/dp/1942788002/ref=sr_1_1?dchild=1&keywords=devops&qid=1603606484&s=books&sr=1-1)

[DevOps: A Software Architect's Perspective by Len Bass, Ingo Weber, Liming Zhu](https://www.amazon.com/DevOps-Software-Architects-Perspective-Engineering/dp/0134049845/ref=sr_1_1?crid=35SVBZXESBH9E&dchild=1&keywords=devops+a+software+architect%27s+perspective&qid=1603606581&s=books&sprefix=devops+architec%2Cstripbooks-intl-ship%2C-1&sr=1-1)

#### Youtube
{{< youtube _Gpe1Zn-1fE >}}

#### Online Courses
[Pluralsight: Understanding DevOps](https://app.pluralsight.com/paths/skills/understanding-devops)

## What is SRE?
Kindly allow me to borrow the definition from Wikipedia and then break it down for better understanding. 

> “Site Reliability Engineering (SRE) is a discipline that incorporates aspects of software engineering and applies them to infrastructure and operations problems.”

At this point I would like to highlight a popular quote from Google - “class SRE implements DevOps”. SRE was developed by Google, in 2003 as a result of few developers maintaining the IT infrastructure. SRE focuses on the reliability of the software.

SRE is said to be a practice and provides various guidelines to achieve reliability, which in turn leads to customer satisfaction. Here the focus is on maintaining a service or system such that it’s highly available, scalable and meets the needs of the end users. When Devops talks about automation, SRE talks about what to automate, how to identify what to automate etc. Explaining SRE requires a separate post in itself. 

To Conclude, understand that SRE is about methods and practices that one team must follow to provide a reliable service. 

### How is it different from DevOps?
When we follow Google's presentations, regularly we can see the below comparison drawn between DevOps and SRE. 

| Devops                             | SRE                        |
| -----------------------------------|----------------------------|
| Reduce organizational silos        | Share Ownership            |
| Accept failure as normal           |  Blamelessness             |
| Implement gradual change           | Reduce cost of failure     |
| Leverage tooling and automation    | toil automation            |
| Measure everything                 | Measure toil & reliability | 

SRE specifically provides methods and tools to meet the goals. For example how to do post mortem (Post incident) analysis?  , How to measure toil so that one can automate the task that is consuming too much of their time in fire-fighting (troubleshooting), How to design SLA,SLO’s so that monitoring KPIs can be set up. Etc. 

### What are the skills required for a SRE engineer?

The skills sought  after in a SRE engineer is that of a developer mindset, who can view the operations as a software engineering problem and develop solutions, so by nature of the job role and practice one needs to have a good grasp of programming principles. I’ve listed them as below 

1. Operations and Software Engineering 
2. Monitoring systems 
3. Automation 
4. System Architecture
5. Troubleshooting & Debugging
6. Culture of trust
7. Incident Management  



### Resources
[Scalyr](https://www.scalyr.com/blog/what-is-sre/)
#### Books
THe below listed books are available freely, published by google. 

[Building Secure & Reliable Systems Best Practices for Designing, Implementing and Maintaining Systems ](https://static.googleusercontent.com/media/landing.google.com/en//sre/static/pdf/Building_Secure_and_Reliable_Systems.pdf)
[The Site Reliability Workbook](https://landing.google.com/sre/workbook/toc/)
[The Site Reliability Engineering](https://landing.google.com/sre/sre-book/toc/index.html)

#### Youtube
{{< youtube  uTEL8Ff1Zvk >}}

#### Online Courses
[ Pluralsight - Site Reliability Engineering Big Picture](https://app.pluralsight.com/library/courses/site-reliability-engineering-big-picture/table-of-contents)

## Difference between System Administrators, DevOps and SRE Engineers
System Administrators, as we know are specialized in one of the IT Infrastructure domains - Hardware, Virtualization, Storage, Networking, Operating Systems etc. DevOps Engineers have the functional knowledge of application as well as IT Infrastructure layer and are bridge between Developers and their IT requirements. On the other hand SRE engineers look at the holistic view of the software systems and services to provide a reliable product to the end users. 

Hope this has given you a general idea. Please feel free to share your comments and feedbacks. 