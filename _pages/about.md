---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
My [Curriculum Vitae](https://github.com/makemebitter/yuhao-cv/raw/master/CV-Yuhao-UCSD.pdf).

I joined Databricks in December 2023, working at the intersection of ML and systems—automation and performance for large-scale distributed systems. I co-own DBSQL workload management and own ML-based predictive costing for all DBSQL queries, turning runtime/cost priors into smarter scheduling, bin-packing, and autoscaling. I also lead LLM-guided auto-evolution of system policies (agent + simulator), and an ongoing foundation-model effort over systems logs to turn platform telemetry into actionable signals for reliability and efficiency. Separately, I co-built QuickPredict, a history-driven prediction service that provides runtime/cost estimates (with confidence) for similar workloads, which the DBSQL scheduler and SQL planner use to improve placement and plan quality.

I received my Ph.D. in Computer Science from [Prof. Arun Kumar's ADALab](https://adalabucsd.github.io/) UC San Diego (2023). My research focused on ML systems, spanning applied ML systems (new capabilities) and systems for ML (infrastructure that makes training faster and more reliable). Highlights include: Panorama (open-vocabulary, high-throughput video recognition via cascaded detection + embedding search), Cerebro / Model Hopper Parallelism (a novel execution mode that increases trial throughput for large-scale model selection), Lotan (large-scale GNN training by decoupling graph data movement from neural compute with partitioning/batching), and the first in-database distributed deep-learning system (multi-node DL directly over DBMS-resident data).

These PhD projects have shipped and influenced industry. Cerebro/Cerebro-DS were open-sourced, incorporated into Apache MADlib, and integrated with VMware Greenplum, enabling external teams (including UCSD public-health researchers) and appearing as third-party tools for Databricks users. These work also helped inspire RapidFire AI, a startup founded by my PhD advisor centered on these ideas.

I received my B.S. in theoretical physics from Nankai University (China) in 2016. I was fascinated by quantum gravity, black holes, and the search for the ‘ultimate truth’-and published two papers from that work.






<!-- On the first front, I worked on a video querying [Panorama system](https://adalabucsd.github.io/panorama.html) for object detection and classification with computer vision and database techniques. On the second front, I have been working on a project [Cerebro](https://adalabucsd.github.io/cerebro.html) that can expedite distributed deep learning by 3x-10x compared to Horovod and TensorFlow Parameter Server.  -->

<!-- I'm also working a lot on bridging data systems (such as Apache Spark, Distributed databases, etc.) with distributed deep learning systems. Some of these works have already been incorporated into the [Apache MADlib](https://madlib.apache.org/) project and adopted&shipped by VMware. In addition to academic conference talks, I also presented the work at the [Spark+AI summit 2020](https://databricks.com/session_na20/resource-efficient-deep-learning-model-selection-on-apache-spark).

I'm always open to opportunities for summer internships.  -->

<!-- short [Resume](https://github.com/makemebitter/yuhao-resume/raw/master/Resume-Yuhao-UCSD.pdf). If you prefer a longer version, I also have a -->
<!-- Currently I am seeking opportunities for summer internship 2020. [My Resume](https://github.com/makemebitter/yuhao-resume/raw/master/Resume-Yuhao-UCSD.pdf) -->


<!-- Research -->
<!-- A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
