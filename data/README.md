# Data

This is the folder that should house the data for your report.

## Raw Data

In the raw data folder should go an unchanged version of the data that you have downloaded from ANES. *You should never change this data!* At this point in the program, we haven't talked about reading from a source table, but there is good practice that you can start now:

> Think of the source data that you're working with as something that you cannot change. In the future, if you have data that is flowing to you in a pipeline, you won't be able to change this upstream pipeline; instead, you'll have to have code written that will ingest and transform to get ready for your models.

## Modeling Data 

The modeling data is the data that you're actually going to use in your report. This might simply have some changes to the names applied to it. Much, much more likely is that it will have to have dropped some observations (take a look into the codebook) and recoded some values from how they are supplied in the raw data.

There is one, and only one thing that must be true: **changes to data that is derived from raw/source data need to be documented in code.**

If you write code that will move your data from `./data/raw/` to `./data/modeling/` then you can both reproduce this change, edit this change, or execute this same set of changes if the raw data were to be updated.

Although there isn't a hard-and-fast rule for the *name* of the code that will make this translation from `./data/raw/` to `./data/modeling/` I often write this cleaning data as a file that is stored in either `./R/` or in `./src/` .
