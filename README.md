# Lab 1

This is the first data lab for UCB MIDS w203.

This is a team-based Lab. Your instructor will either divide you into teams of about three students, or will approve the teams that you have formed. Your goal on this laboratory is to maximize your learning. The best way to accomplish this is to have all teammates engage with every lab component.

We ask that you meet with your teammates as soon as possible to coordinate expectations around working together. To guide your discussion, we have included the team_discussion document for you to fill in as a team. This document is ungraded.

At the end of the lab, we will ask you to submit a short evaluation of your teammates. Note that a single negative review will not affect a student's grade; we may enact a deduction when multiple reviews consistently point to a general problem.

This lab should be submitted to Gradescope. There is one submission slot for your pdf, and another submission slot for your Rmd file. The submissions are set as *group submissions* which means that there should be only one submission per group, with each of the group members associated with that submission. Adding teammates is intuitive, but this [walk-through](https://help.gradescope.com/article/m5qz2xsnjy-student-add-group-members) created by Gradescope can help you if you get stuck.

## Repository Structure 

This repository is structured in a sensible way. It isn't the only way to structure a project, but this is a good starting place that you can modify for your own purposes.

```         
.
├── LICENSE
├── README.md
├── background_literature
├── data
├── lab_1.Rproj
├── prompt
├── renv
├── renv.lock
├── reports
├── sample_answer
├── src
└── team_discussion
```

The `LICENSE` tells people what they can (and cannot) do with this file. The `README.md` tells them what is happening in the project (and this is the file that you're reading right now!). In `background_literature` is content that you might want to read for your project.

`data/` is a folder that contains data that will be used in the project. Inside this folder, there is another file, `./data/README.md` that says more about what is happening in that folder.

`lab_1.Rproj` is a "project file" that helps you to isolate this project from the rest of your work. This is very, very good practice and the way that we've set up the repository relies on you "opening" this project to begin your work.

The prompt that you're responding to is stored in the folder `./prompt/` we'd suggest you read this so that you know what you're supposed to be doing! 😅

The folder `./renv/` contains the files that create the R environment that you're working with for this lab. By using the [renv] package, you're helping to ensure that you can reproduce your work across contributors to the project, and that you will be able to reproduce your work yourself in the future.

The work that you're actually going to produce should be done in `./reports/` . To help you, we've provided a shell document in that folder. Just below that `./reports/` folder is a sample answer, stored in... the folder `./sample_answer/`. You do not need to exactly reproduce this answer, or its format, but it is a reasonable way to approach your solution.

In the `./src/` folder, pronounced "source" are the tools that you might write for yourself to get the project done. One of the main things that I usually have in this folder is a file called something like `clean_data.R` that cleans and structures my data to move it from `./data/raw/` to `./data/modeling/`. The idea behind having this in something like the `./src/` folder is that someone else who comes to the project can anticipate where things might be.

Finally, in this repository is a folder called `./team_discussion/` that gives you some prompting to start off your team's conversations. When are you going to work, how are you going to get things done, and so on and so on.
