## Overview
This document describes the dataset for the paper:

Cartwright, M., Pardo, B. VocalSketch: Vocally Imitating Audio Concepts. In *Proceedings of ACM Conference on Human Factors in Computing Systems* (2015). http://dx.doi.org/10.1145/2702123.2702387

## Abstract
A natural way of communicating an audio concept is to imitate it with one's voice. This creates an approximation of the imagined sound (e.g. a particular owl's hoot), much like how a visual sketch approximates a visual concept (e.g a drawing of the owl). If a machine could understand vocal imitations, users could communicate with software in this natural way, enabling new interactions (e.g. programming a music synthesizer by imitating the desired sound with one's voice). This data set contains thousands of crowd-sourced vocal imitations of a large set of diverse sounds, along with data on the crowd's ability to correctly label these vocal imitations. This data set will help the research community understand which audio concepts can be effectively communicated with this approach. We have released this data so the community can study the related issues and build systems that leverage vocal imitation as an interaction modality.

## Usage
For citations, please use this reference:

Cartwright, M., Pardo, B. VocalSketch: Vocally Imitating Audio Concepts. In *Proceedings of ACM Conference on Human Factors in Computing Systems* (2015). http://dx.doi.org/10.1145/2702123.2702387


## Contact info
Interactive Audio Lab
* http://music.eecs.northwestern.edu

Mark Cartwright
* mcartwright@gmail.com
* http://www.markcartwright.com

Bryan Pardo
* pardo@northwestern.edu
* http://www.bryanpardo.com

## Description of directories
* **vocal\_imitations/included** - This directory contains all of the vocal imitation recordings that met our inclusion criteria and were included in our analysis
* **vocal\_imitations/excluded** - This directory contains all of the vocal imitation recordings that did not meet our inclusion criteria and were not included in our analysis
* **sound\_recordings** - This directory contains the audio files for the referent 'sound recording' audio concepts. NOTE: If you want to obtain the 'everyday' sounds you must obtain them from http://marcellm.people.cofc.edu/confrontation%20sound%20naming/confront.htm since we cannot redistribute them. Use 'everyday_filename_translation.csv' to rename the files to the naming used in this data set.

## Description of the columns of the CSV files
### Column descriptions for sound\_recordings.csv
* **id** - The id of the sound recording
* **sound\_label** - The label associated with the sound recording
* **sound\_label\_id** - The id of the sound label
* **filename** - The filename of the sound recording
* **audio\_concept\_subset** - The audio concept subset from which this sound recording comes

### Column descriptions for sound\_labels.csv
* **id** - The id of the sound label
* **label** - The label for the sound label
* **audio\_concept\_subset** - The audio concept subset from which this sound label comes

### Column descriptions for vocal\_imitations.csv
* **id** - Id of the vocal imitation
* **filename** - Filename of the vocal imitation
* **stimulus\_type** - ('sound label' or 'sound recording') The stimulus type used in the vocal imitation task
* **included** - Boolean of whether this vocal imitation met our inclusion criteria and was used in our analysis
* **draft** - Boolean of whether this vocal imitaiton was a 'draft' vocal imitation
* **training** - Boolean of whether this vocal imitation was for practice and discarded in analysis
* **participant\_id** - The id of the participant who performed the vocal imitation
* **satisfaction** - The participant's satisfaction with their vocal imitation on a 7- level likert scale (*Completely dissatisfied, Mostly dissatisfied, Somewhat dissatisfied, Neither satisfied or dissatisfied, Somewhat satisfied, Mostly satisfied, Completely satisfied*)
* **sound\_label** - The sound label of the audio concept of this vocal imitation (i.e. the stimulus when a stimulus\_type='sound label')
* **sound\_label\_id** - The id of the sound label
* **sound\_recording** - The sound recording of the audio concept of this vocal imitation (i.e. the stimulus when a stimulus\_type='sound recording')
* **sound\_recording\_id** - The id of the sound recording
* **audio\_concept\_subset** - The subset from which the stimulus comes from
* **participants\_sound\_recording\_description** - The participant's description of the stimulus sound recording (if a stimulus\_type='sound recording')
* **participants\_sound\_recording\_description\_confidence** - The participant's confidence in their sound recording description on 5-level Likert scale (*Not at all confident, Not so confident, Neutral, Confident, Very confident*)
* **description\_match** - Boolean of whether participants\_sound\_recording\_description was scored as correct according to the Marcel scoring guidelines (therefore only relevant when audio\_concept\_subset is 'everyday' and 'included' is True and 'stimulus\_type' is 'sound recording'). See paper for more details.


### Column descriptions for identifications.csv
* **id** - Id of the identification
* **identification\_type** - ('sound label' or 'sound recording') The stimulus type used in the vocal imitation task
* **training** - Boolean of whether this identification was for practice and discarded in analysis
* **participant\_id** - The id of the participant that performed the identification
* **vocal\_imitation\_id** - The id of the vocal imitation
* **sound\_label** - The sound label of the referent audio concept for the vocal imitation
* **sound\_recording** - The filename of the sound recording of the referent audio concept for the vocal imitation
* **sound\_label\_id** - The id of the sound label
* **sound\_recording\_id** - The id of the sound recording
* **audio\_concept\_subset** - The subset from which the stimulus concept comes from
* **vocal\_imitation\_filename** - The audio filename of the vocal imitation
* **participants\_vocal\_imitation\_description** - The description the participant (in the identification task) gave for the vocal imitation
* **participants\_vocal\_imitation\_description\_confidence** - The confidence the participant reported having in the description for the vocal imitation on 5-level Likert scale (*Not at all confident, Not so confident, Neutral, Confident, Very confident*)
* **selection\_sound\_label** - The sound label of the participant's choice in forced-choice identification task
* **selection\_sound\_label\_id** - The id of the sound label of the participant's choice in forced-choice identification task
* **selection\_sound\_recording** - The filename of the sound recording of the participant's choice in forced-choice identification task
* **selection\_sound\_recording\_id** - The id of sound recording of the participant's choice in forced-choice identification task
* **selection\_confidence** - The confidence the participant reported having in their forced-choice selection on 5-level Likert scale (*Not at all confident, Not so confident, Neutral, Confident, Very confident*)
* **selection\_match** - Boolean of whether the forced-choice selection was correct
* **distractor0\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor1\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor2\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor3\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor4\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor5\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor6\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor7\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **distractor8\_id** - The id of one of the distractor sound recording or sound label (depending on the identification\_type)
* **description\_match** - Boolean of whether participants\_vocal\_imitation\_description was scored as correct according to the Marcel scoring guidelines (therefore only relevant when audio\_concept\_subset is 'everyday'). See paper for more details.


### Column descriptions for participant\_survey.csv
* **participant\_id** - The id of the participant
* **age** - The reported age of the participant
* **gender** - The reported gender of the participant
* **hearing\_problems** - The participant's response to the question: "Have you ever been diagnosed with a hearing problem?"
* **speech\_problems** - The participant's response to the question: "Have you ever been diagnosed with a speech problem?""
* **years\_actively\_using\_music\_tech** - The participant's response to the question: "Estimate (in years and months, e.g. 5 years 2 months) how long you have been actively using ﻿audio/music production technology (e.g. recording, mixing, synthesis technology)."
* **frequency\_using\_music\_tech** - The participant's response to the question: "How frequently do you use audio/music production technology (e.g. recording, mixing, synthesis technology)?" (*Never, Less than once or twice a year, Once or twice a year, Once or twice a month, Once or twice a week, More than once or twice a week*)
* **years\_actively\_making\_music** - The participant's response to the question: "Estimate (in years and months, e.g. 5 years 2 months) how long you have been actively creating, practicing, or performing music."
* **frequency\_making\_music** - The participant's response to the question: "How frequently do you create, practice, or perform music?" (*Never, Less than once or twice a year, Once or twice a year, Once or twice a month, Once or twice a week, More than once or twice a week*)
* **years\_actively\_singing** - The participant's response to the question: "Estimate (in years and months, e.g. 5 years 2 months) how long you have been actively singing."
* **frequency\_singing** - The participant's response to the question: "How frequently do you sing?" (*Never, Less than once or twice a year, Once or twice a year, Once or twice a month, Once or twice a week, More than once or twice a week*)


### Column descriptions for 'everyday_filename_translation.csv'
This CSV file is for translating the filenames from the Marcel data set to the file naming convention used in this dataset.
* **marcel_filename** - The name of the file in the Marcel data set
* **vocalsketch_filename** - The name of the file when used in the VocalSketch data set