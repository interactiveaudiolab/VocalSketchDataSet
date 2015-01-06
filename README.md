## Overview
This document describes the dataset for the paper "VocalSketch: Vocally Imitating Audio Concepts"

## Description of directories
* included_vocal_imitations - This directory contains all of the vocal imitation recordings that met our inclusion criteria and were included in our analysis
* excluded_vocal_imitations - This directory contains all of the vocal imitation recordings that did not meet our inclusion criteria and were not included in our analysis
* sound_recordings - This directory contains the audio files for the referent 'sound recording' audio concepts. NOTE: If you want to obtain the 'everyday' sounds you must obtain them from http://marcellm.people.cofc.edu/confrontation%20sound%20naming/confront.htm since we cannot redistribute them.

## Description of the columns of the CSV files
### Column descriptions for sound_recordings.csv
* id - The id of the sound recording
* sound_label - The label associated with the sound recording
* sound_label_id - The id of the sound label
* filename - The filename of the sound recording
* audio_concept_subset - The audio concept subset from which this sound recording comes

### Column descriptions for sound_labels.csv
* id - The id of the sound label
* label - The label for the sound label
* audio_concept_subset - The audio concept subset from which this sound label comes

### Column descriptions for vocal_imitations.csv
* id - Id of the vocal imitation
* filename - Filename of the vocal imitation
* stimulus_type - ('sound label' or 'sound recording') The stimulus type used in the vocal imitation task
* included - Boolean of whether this vocal imitation met our inclusion criteria and was used in our analysis
* draft - Boolean of whether this vocal imitaiton was a 'draft' vocal imitation
* training - Boolean of whether this vocal imitation was for practice and discarded in analysis
* participant_id - The id of the participant who performed the vocal imitation
* satisfaction - The participant's satisfaction with their vocal imitation
* sound_label - The sound label of the audio concept of this vocal imitation (i.e. the stimulus when a stimulus_type='sound label')
* sound_label_id - The id of the sound label
* sound_recording - The sound recording of the audio concept of this vocal imitation (i.e. the stimulus when a stimulus_type='sound recording')
* sound_recording_id - The id of the sound recording
* audio_concept_subset - The subset from which the stimulus comes from
* participants_sound_recording_description - The participant's description of the stimulus sound recording (if a stimulus_type='sound recording')
* participants_sound_recording_description_confidence - The participant's confidence in their sound recording description

### Column descriptions for identifications.csv
* id - Id of the identification
* identification_type - ('sound label' or 'sound recording') The stimulus type used in the vocal imitation task
* training - Boolean of whether this identification was for practice and discarded in analysis
* participant_id - The id of the participant that performed the identification
* vocal_imitation_id - The id of the vocal imitation
* sound_label - The sound label of the referent audio concept for the vocal imitation
* sound_recording - The filename of the sound recording of the referent audio concept for the vocal imitation
* sound_label_id - The id of the sound label
* sound_recording_id - The id of the sound recording
* audio_concept_subset - The subset from which the stimulus concept comes from
* vocal_imitation_filename - The audio filename of the vocal imitation
* participants_vocal_imitation_description - The description the participant (in the identification task) gave for the vocal imitation
* participants_vocal_imitation_description_confidence - The confidence the participant reported having in the description for the vocal imitation
* selection_sound_label - The sound label of the participant's choice in forced-choice identification task
* selection_sound_label_id - The id of the sound label of the participant's choice in forced-choice identification task
* selection_sound_recording - The filename of the sound recording of the participant's choice in forced-choice identification task
* selection_sound_recording_id - The id of sound recording of the participant's choice in forced-choice identification task
* selection_confidence - The confidence the participant reported having in their foreced-choice selection
* selection_match - Boolean of whether the forced-choice selection was correct
* distractor0_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor1_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor2_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor3_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor4_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor5_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor6_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor7_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)
* distractor8_id - The id of one of the distractor sound recording or sound label (depending on the identification_type)


### Column descriptions for participant_survey.csv
* participant_id - The id of the participant
* age - The reported age of the participant
* gender - The reported gender of the participant
* hearing_problems - The participant's response to the question: "Have you ever been diagnosed with a hearing problem?"
* speech_problems - The participant's response to the question: "Have you ever been diagnosed with a speech problem?""
* years_actively_using_music_tech - The participant's response to the question: "Estimate (in years and months, e.g. 5 years 2 months) how long you have been actively using ﻿audio/music production technology (e.g. recording, mixing, synthesis technology)."
* frequency_using_music_tech - The participant's response to the question: "How frequently do you use audio/music production technology (e.g. recording, mixing, synthesis technology)?"
* years_actively_making_music - The participant's response to the question: "Estimate (in years and months, e.g. 5 years 2 months) how long you have been actively creating, practicing, or performing music."
* frequency_making_music - The participant's response to the question: "How frequently do you create, practice, or perform music?"
* years_actively_singing - The participant's response to the question: "Estimate (in years and months, e.g. 5 years 2 months) how long you have been actively singing."
* frequency_singing - The participant's response to the question: "How frequently do you sing?"