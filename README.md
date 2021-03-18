# Project-Template
Template for research projects

Writing scientific papers is hard. This project template is my attempt at making it no more header than it needs to be hopefully, it allows us to focus more on doing science and less on file management, finding templates, finding models, knowing what comes next, etc.

## The structure

The **admin** folder includes all administrative documents, such as IRB and PreRegistrations

The **materials** folder is destined to hold all instruments, qualtrics qsf files, and all you might need to replicate the study or run a variation.

The **data** folder, well, holds all of your raw data. Please, do not manually edit data files. Do all such editing in R, so that. If you get more data, you don't need to re-do all those steps. Filtering, variable naming,  exclusions, etc, should be done reproducibly through R.

The **analysis** folder holds all R files, be they scripts or markdowns.

The **output** folder holds R output. RDA and RDS files go in the home folder; plots, tables and reports have their own.

Finally, the **submission** folder holds all submission related files: letters to the editor, journal proofs, etc.

## The home folder

... holds a Homebase file, where you can link all relevant files, and important information. One of the benefits of google drive, is that you can rely on hyperlinks to find what you want faster, so feel free to link to your hearts content; or not.

The original Madlibs template, the first step often required before running a study in the Duckworth Lab.

The manuscript itself. Two templates are provided (multistudy vs. single-study), keep the one you'll use.

The master R file. The idea behind this is that this file does all the reproducible steps needed to go from raw data to finalized report. This way, if you change something in the analysis files,  if the data files are updated, etc. you can just re-run the master file so the dat is cleaned, exported, re-read, analyzed, and piped into reports (html, presentation, pdf, manuscript, etc).

The R project file, which is useful for managing working directories, and keeping everything organized.

A To-Do file, which include the (generalized) steps you need to take in the order you probably need to take them to achieve your goal of publishing your paper. It includes a backwards planning template.

## Google Docs vs. Rmarkdown

Rmarkdown is great at reproducibility, but somewhat sucks to get feedback. Google docs is the opposite. How do we fix this conundrum. Two alternatives.

1. Write in google docs, when including tables and figures, link them to the relevant google drive, so that they will be automatically updated should those files change. Only images update, so (1) save tables as images, (2) any statistical information in text will need to be updated manually.

(OR - My preferred alternative)

2. Write in Rmarkdown. When you are ready to get feedback, copy from the html file into word/google doc. Get feedback *with tracked changes*, so that after you get it, you can incorporate that feedback into your RMmarkdown without breaking your reproducibility.

## Other integrations

**Important Warning** Beware of making private data public!

Every project can (should?) have its respective GitHub Repo, OSF project, and folder within Zotero reference management.

**Github.** It's nice to see your contributions. I feel like seeing your commit chart getting greener and greener might be a good way to stay motivated.

**OSF.io** Hosts pre-registrations and Pre-prints, so it may be a good idea to integrate into the workflow.

**Zotero** Is the only reference manager that is integrated into RStudio,  making keeping track of references a breeze.

## Useful R packages to check out

- papaja allows you to use Latex to typeset journal submissions and to format papers in nice double columns APA style formatting.

- rticles is another alternative to that.
