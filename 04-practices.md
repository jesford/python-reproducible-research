---
layout: page
title: Reproducible Research
subtitle: Best Practices
minutes: 10
---
> ## Learning Objectives {.objectives}
>
> * Know that a license is required for code to be reused.
> * Be able to give an example of an open source license.
> * Know that Zenodo is a website for archiving data.
> * Describe at least one tool or technique for enabling reproducibility on a large scientific research projects (*examples:* packaging, testing, continuous integration, modular code, **others to include?**).

In the last activity we gained some experience attempting to publish a reproducible workflow, and in trying to follow along with the analysis of another group. In academic research it is often the case that we are collaborating with or building off of the results of a researcher at a different institution, with whom we cannot just turn to and ask questions. We practiced creating a GitHub Issue as a way to ask questions or suggest improvements to a project.

> ## How did it go? {.challenge}
>
> What did you learn in trying to create a reproducible result, and then reproducing
> what someone else had done? What worked well? Can you give examples of things that
> made code easy or difficult to understand? What would you do differently next time?
> Did anyone add a License?

The idea that simply putting code on the internet gives other people the right to use it is a misconception. *Licenses are required in order for code to be reused!* Websites such as [choosealicense.com](http://choosealicense.com/) can help you pick a license to match your specific needs.

> ## Choose a License {.challenge}
>
> Add a license to your project repository, if it doesn't already have one. An
> example of a nice and simple permissive license is the 
> [MIT license](http://choosealicense.com/licenses/mit/). If you have already 
> done this, choose a software tool that you use in your research (or that we have
> covered in this workshop) and find out what kind of license it has.

The reproducible workflows we created today were very short compared to most scientific analyses. When a project becomes larger, extra care must be taken to keep it organized and useable for others. Some of the topics that we have already covered are breaking our code into reuseable pieces like functions, and including Docstrings, comments, and README files for documentation.
