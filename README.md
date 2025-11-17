# DataManagement
Some of my acquired systems for improving data management and record-keeping.

## It all runs because of the "mkdir" line of code

Adapt the following code to create a multi-level document for each new experiment:

mkdir -p ~/OneDrive/RothJacob_PhDFiles/1-Projects/2-Experiments/JSRe0002-T_Cellular-WB_NB02-153_Chromatin analysis of PRMTi cells: titration of KCl for fractionation validation/{1-notes,2-data_raw,3-code,4-data_processed,5-figures}

If you utilize an InventorySheet, all you need to do is enter the data for each new experiment into the excel file and the mkdir code is concatenated:
1. copy this code from the excel file
2. hit "cmd+spacebar" on mac to open the terminal
3. paste and execute code
4. observe new folder set for your experiment

## My unique ID system
Ubiquitiously throughout all of my projects, I include these unique naming schemas:

### JSRe####-T_
- “Top” folder for any given experiment; useful to search “JSRe####-T” for any experiment to immediately navigate to an experiment of interest
  - I also utilize "cmd+up/down arrow" and "option+up/down arrow" all the time to navigate my folders (on a mac). I hate clicking with a mouse.

### JSRe####-R_
- “Results” file; useful to search “JSRe####-R” for any experiment to immediately navigate to the summary results of an exp. This is so helpful when talking to my PI and I want to quickly pull up the digital results of an experiment to show him in lab meeting.
- Once I have found that file, the filename will also have the NB##-### reference number to immediately navigate to the relevant physical NB page. If coded into Rmd file, better to have png vs pdf images for viewing, but I recommend saving results in both formats.

### JSRg###
- Any gel I have ever run has a unique ID; agarose gels, western blots, Coomassie stains, everything. Massively simplifies keeping track of western blots as well. Save this name with every image for the named gel (along with the experiment number)

### JSRp###
- Any plasmid I’ve ever collected/created

### JSRi###
- Any oligo I order: primers/DNA sequences, RNA, etc

### JSRs####
- Immunofluorescence slides; I add more meta data to each slide, with with this code + an excel file with the metadata, a singular annotation on a slide is sufficient to communicate all data (so long as excel file is updated and you use an EtOH-resistant marking device)

### JSRe####-I_
- How I start the name of any “Illustrator” file that is processing data for an experiment; useful to search “JSRe####-I” for any experiment to immediately navigate to an adobe illustrator data sheet of interest.

### JSRe####-G_
- Graphpad Prism file for a project



## Protocol naming
All protocol saved file names start with a “P_” call so that I can search for them quickly. In my protocols folder I keep a living/continuously updated protocol (save archived versions with appended date for when they were archived into an "archive" subfolder). Then when I use it for an experiment I copy it into the “1-notes” folder for that particular experiment folder, renaming it “JSRe####-P_...” to enable me to rapidly search and pull up the protocol for that exp, as well as see any new changes I made to the protocol for that experiment.


## Using the rmd file to create a living document of what you're currently working on
After growing incredibly tired of wasting time formatting and reformating a powerpoint for each check-in meeting with my PI, I created a living rmd document that includes my main objectives at that time, highlights what we need to talk about at the meeting, and dynamically updates with the experiments I want to focus on for a particular meeting based on the status in my InventorySheet.

See the example in this repo, with a template InventorySheet and example results image.

Since the rmd only knits together the experiments that I want to include, I can retain all entries for historical experiments and always explore the rmd file for the most recent developments for each experiment.

