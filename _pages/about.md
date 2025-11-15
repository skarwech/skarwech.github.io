---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


Welcome — I'm Abderrahim Akhrouf, a PhD candidate in Fluid Mechanics. I build machine learning models and apply electrical impedance tomography to improve pump energy efficiency and real-time monitoring. On this site you'll find research summaries, publications, teaching materials, a curated CV, and datasets associated with the thesis.

<div class="hero">
  <div class="container">
    <h1 class="hero__title">Optimizing energy consumption in electric pumps</h1>
    <p class="hero__subtitle">Combining electrical impedance tomography with machine learning to monitor and optimize pump performance. Explore the thesis summary and code below.</p>
    <a class="btn btn--primary" href="{{ site.baseurl }}/thesis/" aria-label="Read thesis">Read Thesis</a>
    <a class="btn btn--inverse" href="{{ site.baseurl }}/publications/" aria-label="Open publications">Publications</a>
    <a class="btn" href="mailto:abderrahim.akhrouf@etu.univ-amu.fr" aria-label="Contact by email">Contact</a>
  </div>
</div>

Featured — Thesis and Research
------------------------------

My doctoral research focuses on optimizing electric pump operation using data-driven control with EIT-based sensing and advanced ML models. If you're interested in the project, click the `Thesis` link in the top menu for the abstract, key results, and downloadable resources.

Recent work and tools
---------------------

- EIT preprocessing pipeline (open-source Python notebooks) — data cleaning, forward simulation, and reconstruction
- ML models for anomaly detection and pump optimization — reproducible code and trained models
- Conference papers and a preprint summarizing results (see `Publications`)

Contact
-------

If you'd like to collaborate or inquire about supervision, email me at: `abderrahim.akhrouf@etu.univ-amu.fr` or connect on LinkedIn.

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual Markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the Markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and Markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
