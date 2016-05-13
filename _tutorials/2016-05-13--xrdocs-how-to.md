---
published: true
date: "2016-05-13 16:35 +0530"
title: "@xrdocs How-To"
permalink: "/tutorials/xrdocs-how-to"
author: Akshat Sharma
excerpt: "This tutorial provides a walkthrough of the xrdocs platform for blogging, and creating tutorials and techdocs"
tags: 
  - iosxr
  - cisco
position: " "
---

Welcome to @xrdocs!

This tutorial is meant to get a new blogger/technical-writer, unfamiliar with @xrdocs, up and running in minutes.

Cisco IOS-XR 6.0+ brings with it some key operational enhancements in the domains of monitoring, automation, application-hosting and software management. However, these enhancements require the right tools to aid their consumption. 

In our minds, at a macro level we can classify the tools into two types:

* **User end tools/applications**:  eg. YDK-py, Streaming Telemetry plugins for ELK/Prometheus/SignalFX, support for Config-management tools like Ansible, Puppet and Chef, YUM repositories for WRL7 apps etc.
* **Documentation**: Regular Blogs, Step-by-step tutorials and detailed technical documents have to accompany tools. There is probably nothing more infuriating than a badly documented piece of code/tool/feature.
  
  
  
**@xrdocs** has been designed to address these documentation concerns. 
{: .notice--warning}


>
*   We needed a platform to quickly churn out relevant documentation and make sure it remains up-to-date with all the changes coming up in IOS-XR. 
*   We wanted to peer-review our documentation, raise bugs against it and give control directly to the technical writers. In short, we wanted to treat documentation like code.
{: .notice--info}




The choice was simple: If you've followed the tremendous success of github-pages ever since its inception, it would be clear that using [github](https://github.com) as a platform to host and edit our documentation-as-code, was the way to go.

So here we are, @xrdocs is up and running at <https://xrdocs.github.io> with links to domains of interest.
{: .notice--success}


Woah! but wait. Not everyone is comfortable dealing with code while documenting. And really? git workflows each time you need to push a document? Is there an easier way? 
Read on.


## Introducing [prose.io](http://prose.io)

We've completely abstracted the internals of the website running on github-pages using [prose.io Config](https://github.com/prose/prose/wiki/Prose-Configuration) configurations.


> 
Now all you need is:
>
*   A github account. If you don't have one, get it here: [Join Github](https://github.com/join)
*   A relatively new browser (chrome would be recommended). (No IE please!)
*   A link explaining markdown syntax if you've never used it: [Markdown Cheat-Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
{: .notice--warning}

[prose.io](http://prose.io) is a simple markdown editor that is built with [backbone.js](http://backbonejs.org/) and has deep integrations with github.

>
Advantage?
>  
If all you want to do is create a new document/blog, you don't need to use git workflows anymore. No more cloning of repos, no more git pull, merge, push to keep your local account up to date. Just open up your the relevant location in [prose.io](http://prose.io) and start writing in markdown.




### Authorize [prose.io](http://prose.io) with your github account


Browse to  [prose.io](http://prose.io) and if you've never authorized it before, you'll be presented with the following page:

![Box validation](https://xrdocs.github.io/xrdocs-images/assets/tutorial-images/proseio_authorize.png)
Click on **Authorize on Github** and you'll be taken to the Github login screen. When you login, allow prose.io to access your public and private github repos (don't worry, this is a purely client side js app).
{: .notice}


![Box validation](https://xrdocs.github.io/xrdocs-images/assets/tutorial-images/authorise_github.png)
Click on **Authorize Application**
{: .notice}


Now the page will automatically redirect to show the home page repositories for the user:
![Box validation](https://xrdocs.github.io/xrdocs-images/assets/tutorial-images/proseio_authorized_home.png)



















