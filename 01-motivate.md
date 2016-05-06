---
layout: page
title: Reproducible Research
subtitle: Motivating Reproducibility
minutes: 10
---
> ## Learning Objectives {.objectives}
>
> * Describe why reproducibility and openness is good for science
> * Explain how a reproducible workflow benefits an individual researcher
> * Know the purpose of a README file

Isaac Newton famously [said](https://en.wikiquote.org/wiki/Isaac_Newton) "If I have seen further it is by standing upon the shoulders of giants." Science progresses by building upon past knowledge to design experiments and make new discoveries. When previous results are easy to build upon, new results can be obtained faster with less effort. 

> ## Its not always easy to build off past work... {.challenge}
>
> Can you give an example of a time you had difficulty understanding how a previous 
> result was obtained? Did a journal article forget to give all the pertinent details? 
> Have you ever had to re-do an experiment (or re-write some code) that someone else 
> had previously done? Did you feel that it was a productive use of your time?

Unfortunately, scientists can spend a lot of their time reinventing the wheel, meaning that they are simply trying to re-do what someone else has done in order to take the analysis one step further or in a different direction. But it doesn't have to be this way! By learning to write good code and using version control, you now have some of the essential tools for doing reproducible research. In fact, by simply opening your Jupyter Notebook from the earlier Python lesson, you could quickly and easily reproduce all of our discoveries about that suspicious inflammation data.

The selfish reasons to be reproducible, examples of case studies in increased productivity?

> ## Dangers of Non-reproducibility {.callout}
>
> Examples of some [retracted papers](), because results were not reproducible.

An essential piece of creating reproducible research is clearly documenting what you have done. One way to document your research is by writing papers, but it is usually impossible to give *all* of the details, especially if there is programming involved. Some useful documentation techniques that we have already covered are using comments in your code, and attaching Docstrings to your Python functions.  

The Jupyter Notebook is a great tool for reproducible research because the cells naturally lend themselves to a step-by-step process which anyone else with a copy can execute. The notebook also has nice built-in support for documenting the procedure, through the use of Markdown cells. Let's see how this works. Navigate to the directory from the previous Python lesson, where we saved our Jupyter Notebook for analyzing patient inflammation data. Let's open that notebook and add some Markdown documentation.

~~~ {.bash}
$ cd ~/Desktop/data
$ jupyter notebook
~~~

After selecting and opening an existing notebook, create a new cell at the very top. Go to the dropdown menu on the toolbar that currently says "Code", and change it to select "Markdown". Notice that the number next to the cell disappears -- this cell will no longer be interpreted as a block of code to execute. Inside of the cell, type the following lines and then execute the cell. 

~~~ {.python} 
# Arthritis Study
An analysis of inflammation data.

### Details:
- Study duration: 40 days
- Number of patients: 60

*Note: this data has some suspicious features! Remember to follow up with the data collection team.*
~~~

> ## Tips {.callout}
>
> Use the `+` button in the toolbar to create a new cell (it will appear underneath 
> whichever cell is currently highlighted). Use the up and down arrows in the toolbar 
> to move the cell to the desired position.

Our Markdown cell gets nicely rendered by the Jupyter Notebook, with different size headers, bullet points and italicized text (many more [options](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) are available). It can be useful to add frequent Markdown cells to a notebook, to explain your thought process and the steps of analysis, and to keep track of notes to yourself.

> ## Document a step {.challenge}
>
> Create another Markdown cell, anywhere in the notebook. Include some notes about
> the analysis or results.

A final important way to document the use of some code is to create a README file. A README explains the contents of a directly as a whole, not just a single file, and describes how the things in the directory fit together to achieve their intended purpose. A good README contains all the instructions necessary to use the code, data, and any other elements of a self-contained research project.

> ## Create a Simple README file {.challenge}
>
> Let's now create a README file for this directory, using the same Markdown language
> that we used for formatted text in the Jupyter Notebook. 
>
>`$ nano README.md` 
>
> The `.md` extension is not required, but it is the convention for a Markdown file. 
> We could also have created a plain text `.txt` file instead.
> (provide a fill-in-the-blanks sample README)
>
> Compare your README to your neighbors. What other information might be useful to include?

~~~ {.bash}
$ nano README.md
~~~
