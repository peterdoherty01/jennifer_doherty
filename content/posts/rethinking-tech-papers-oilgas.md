+++
date = "2019-02-22"
title = "Rethinking Technical Papers in Oil & Gas"
slug = "rethinking-tech-papers-oilgas"
tags = ["jupyter","markdown","conference","technical","collaboration"]
categories = ["startup","computation-hub","oil","energy"]
+++
<center>
![](/posts/post_pics/laptop-3174729_640.jpg)
</center>
## Motivation

The way in which engineers report and publish technical papers hasn't changed much over the past several decades.

At Computation Hub, we have peer-reviewed some novel work involving Machine Learning to be considered for a conference. It got us thinking about the whole review process when we checked the paper.

One of the main reasons to publish work at a conference is to share knowledge so that it can benefit others in the industry. The main issue that I find is that one cannot easily take the work presented, validate it, test it or build upon it. Basically, I cannot copy and paste algorithms into the format I'd like to work in e.g. Python (Jupyter Notebook) or R.

## Fast Forward

Normally, engineers use tools like Excel or Python to analyze data, generate results and create plots and tables for reporting. These results are then transferred as tables and figures into Word documents. This is **a painful, manual way** to 1) perform analysis and 2) validate work as from a quality control perspective. Errors will always persist with this method.

A **data-driven culture** within Oil & Gas is recognized as being key to unlocking the future of the industry. Thanks to research by [Alfonso R. Reyes](https://www.linkedin.com/pulse/evolution-data-science-machine-learning-artificial-petroleum-reyes/), we can deduce that Python and R are the languages increasingly used amongst engineers for Machine Learning and Data Science. Furthermore, more and more papers are being published with Machine Learning and Data Science methodologies. It can also be deduced from the popularity of open online courses and competitions proposed by [Kaggle](https://www.kaggle.com/), that new engineers to the industry prefer working with these languages.

**A streamlined way** to make papers more useful to your organization and the industry is required. Performing data analysis and presenting results tables and figures in one centralized place is a good solution. This could be done with Jupyter Notebooks and **source control (e.g. GitHub)**. When ready for publication, one can compile the notebook for PDF or other format (e.g. .html). Thus, reducing hard labour, which nobody wants.

## Getting On Board

Is a big effort required to adopt this method? No. Simply put, the industry already uses languages like Python and R for their analysis work anyway. Writing reports in this way does not require a big upheaval in any way.

I haven't looked at all the limitations but some barriers could be workforce age and culture. People may be "set in their ways" after 20, 25 years in the industry. Why would I change an established format now?

Currently, in the draft template proposed (See next section), there is no automatic figure or table numbering. But this might be addressed by using LaTex - I don't believe it's a showstopper. Moreover, if another markup format is used, PanDoc or a similar tool could be a solution to offer a **zero cost alternative** to current methods.

**One more reason** to get on board with this idea is that it's compelling for new engineers to the industry. New recruits and seasoned professionals are already upskilling with these tools. **Second**, it offers a truly collaborative channel among team members to ensure a quality paper is proposed for publication. Focusing on the content instead of repetitive, manual tasks such as copying and pasting into Word is something to be considered.

## Example Template - A Way Forward

To get a clearer picture of what I'm discussing in this article, I've set up an [example Jupyter Notebook draft template](https://nbviewer.jupyter.org/github/peter-doherty/oil_gas_technical_paper_templates/blob/master/python/Technical_Paper_Template_Oil_Gas.ipynb). It could be adapted for R too. These notebooks, when ready for publication could be easily put behind a paywall to maintain revenue channels for the conference organizers.

The source repository can be found and updated via [GitHub](https://github.com/peter-doherty/oil_gas_technical_paper_templates) and is **open to contributions** from the industry.

**The idea is to allow the industry to build upon this template through open collaboration under the GNU General Public License v3.0.**

## Conclusion

You might be asking yourself: "Does any other industry do this?". The short answer is yes.

I've gathered some **examples from the Finance, Mathematical and Scientific communities** hereafter:

*   Finance: [https://nbviewer.jupyter.org/github/vincentarelbundock/Reinhart-Rogoff/blob/master/reinhart-rogoff.ipynb](https://nbviewer.jupyter.org/github/vincentarelbundock/Reinhart-Rogoff/blob/master/reinhart-rogoff.ipynb)

*   Mathematics: [https://nbviewer.jupyter.org/github/fonnesbeck/multilevel_modeling/blob/master/multilevel_modeling.ipynb](https://nbviewer.jupyter.org/github/fonnesbeck/multilevel_modeling/blob/master/multilevel_modeling.ipynb)

*   Physics: [https://nbviewer.jupyter.org/github/waltherg/notebooks/blob/master/2013-12-03-Crank_Nicolson.ipynb](https://nbviewer.jupyter.org/github/waltherg/notebooks/blob/master/2013-12-03-Crank_Nicolson.ipynb)

This idea is not a "game changer" for the industry. But, as working in the browser becomes more mainstream in Oil & Gas, programming in the browser to report our learnings should be adopted too. An improvement like this, with not-so-much effort, can contribute to:

1.  Boosting the quality of the industries work
2.  Encouraging young engineers to publish their work
3.  A reduction of boring, repetitive tasks

By adopting a practice like the one proposed, can open up the industry to new ideas and inspire young engineers to build for the future.

## Further Reading

1.  [Intro to Anaconda](https://www.anaconda.com/)
2.  [Intro to Jupyter Notebooks](https://www.youtube.com/watch?v=q_BzsPxwLOE)
3.  [Intro to R](https://www.youtube.com/watch?v=DNS7i2m4sB0)
4.  [Publishing Jupyter Notebooks, Documentation](https://ipypublish.readthedocs.io/en/latest/)
5.  [A Gallery of interesting Jupyter Notebooks](https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks)
6.  [A Gallery of interesting Jupyter Notebooks in languages other than Python](https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks#notebooks-in-languages-other-than-python)
7.  [Markdown Explanation](https://en.wikipedia.org/wiki/Markdown)
8.  [Rmarkdown Journal templates](https://github.com/rstudio/rticles/tree/master/inst/rmarkdown/templates/rjournal_article)
9.  [Rstudio Gallery](https://rmarkdown.rstudio.com/gallery.html)

## Share Your Thoughts & Contribution

Did you find this article interesting? If you're interested in supporting or contributing to this proposal please contact me at: peter@computationhub.com. By doing so, it would help move this idea to the next step and to the attention of ASME, OTC and other industry parties.)

This post was originally posted here: [https://computationhub.com/blog/2019/02/21/rethinking-technical-papers-oil-gas/](https://computationhub.com/blog/2019/02/21/rethinking-technical-papers-oil-gas/)