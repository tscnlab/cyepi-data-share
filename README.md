# Experiment background

| Dataset name | cyepi |
| --- | --- |
| Period of data collection (total) | August 2023 to November 2023 |
| Location | Tübingen, Germany |
| Number of participants enrolled  | N=30 |
| Number of participants included in data analysis and this repository | N=26 |
| Duration of experiment for each participant | N=7 days (Monday to Monday) |

The aim of the experiment was to characterise personal light exposure centrally at the near-corneal level. For this, participants wore an ActLumus light logger mounted centrally on non-prescription glasses for the entire duration of the experiment. Additionally, they wore an ActTrust2 actimeter at the wrist level for the entire duration of the experiment to measure their activity. 

| Wearable device | Temporal resolution |
| --- | --- |
| ActLumus | 10 seconds |
| ActTrust2 | 60 seconds |

Throughout the week, participants had to complete several questionnaires aimed at understanding the contextual and psychological factors contributing to their light exposure. 

REDCAP - MyCap

# Structure of the folders

## Group

This folder contains grouped data, i.e. any data that are collected at the group level and/or were grouped to facilitate import during analyses.

| File | Description | Corresponding questionnaire |
| --- | --- | --- |
| actlumus | N=26 files from ActLumus, one for each participant | N/A |
| acttrust | N=26 files from ActTrust2, one for each participant | N/A |
| chronotype | N=2 csv files, one for the meq questionnaire and one for the mctq questionnaire. Each contains data for all participants.  | Munich Chronotype Questionnaire (MCTQ) and Morning Eveningness Questionnaire (MEQ). |
| demographics | N=2 csv files. “201_231_demog_20231123.csv” contains only demographic information for N=26 participants. “201_231_demog_health_20231123.csv” contains both demographic as well as health information for N=26 participants. | Custom screening questionnaires. |
| discharge | N=1 csv file, which contains answers from all N=5 questionnaires that N=26 participants had to fill at discharge. | 1) Light Exposure Behaviour Assessment (LEBA) instrument, 2) Visual Light Sensitivity Questionnaire 8 (VLSQ-8), 3) Assessment of Sleep Environment (ASE) questionnaire, 4) Modified Theory Framework of Acceptability (mTFA) questionnaire, 5) Feedback (1 Y/N and 6 multiple choice questions). |
| sleepdiary | N=26 csv files, each corresponding to the sleep diary of an individual participant.  | Core Consensus Sleep Diary.  |
| wearlog | N=26 csv files, each corresponding to the wear log participants filled multiple times/day. | Custom questionnaire.  |

## Individual

This folder contains individual-level data for N=26 participant, each stored in a separate folder named after the participant ID (e.g. 201, 202 etc.). Furthermore, it also contains a folder where the ActLumus files for the environmental light light logger (named “ambient”) are stored. The data within each participant folder follows the following structure. 

| Folder name | Filename (sample) | Description and frequency | Questionnaire naming on REDCap | Coding of questionnaire | Notes |
| --- | --- | --- | --- | --- | --- |
| chronotype | PID_mctq_yyyymmdd.csv | Munich Chronotype Questionnaire (MCTQ) completed at study intake (Monday, day 1) |  |  |  |
| chronotype | PID_meq_yyyymmdd.csv | Morning Eveningness Questionnaire (MEQ) completed at study intake (Monday, day 1) |  |  |  |
| continuous/actlumus/ | PID_actlumus_Log_automatedtimestamp.txt | ActLumus data, collected continuously (every 10 seconds) over the 8 days | N/A | N/A |  |
| continuous/actlumus/ | PID_actlumus_Log_automatedtimestamp_Report.txt | N/A. This is a automated report which is saved with the actual data.  | N/A | N/A |  |
| continuous/acttrust/ | PID_acttrust_Log_automatedtimestamp.txt | ActTrust2 data, collected continuously (every 60 seconds) over the 8 days | N/A | N/A |  |
| continuous/acttrust/ | PID_actlumus_Log_automatedtimestamp_Report.txt | N/A. This is a automated report which is saved with the actual data.  | N/A | N/A | This is missing for PID 202 and PID 204 |
| continuous/currenconditions | PID_currenconditions_yyyymmdd.csv | Questionnaire comprising 3 questionnaires on 1) current mood (MoodZoom), 2) light conditions (custom) and 3) alertness (Karolinska Sleepiness Scale). Completed 4/times per day, at 11:00, 14:00, 17:00 and 20:00. Participants instructed to completed as close as possible to the indicated times.  | Current conditions (4 times/day) |  |  |
| continuous/exercisediary | PID_exercisediary_yyyymmdd.csv | Custom made questionnaire on exercise. Completed daily in the evening | Custom made  |  |  |
| continuous/experiencelog | PID_experiencelog_yyyymmdd.csv | Custom made questionnaire about experiences wearing the light glasses. Completed any time participant had an experience to report (no restrictions). | Custom made |  | Empty folder for PID 210 and 225 |
| continuous/mHLEA_digital | PID_mHLEA_digital_yyyymmdd.csv | Custom made questionnaire to test Daily in the evening | Custom made |  |  |
| continuous/mHLEA_paper | PID_mHLEA_paper_yyyymmdd.xlsx | N/A. This was transcribed by the experimenter after study end for each participant.  | N/A |  | For PID 218 to 231, this includes not only light exposure but also hourly self-reported activity. |
| continuous/mHLEA_paper/upload | jpg, png or heic files from participants phones that were sent to experimenter during the week, later transcribed into the PID_mHLEA_paper_yyyymmdd.xlsx file | Daily in the evening |  |  | This folder is only present for PID 216 to 231. |
| continuous/sleepdiary/ | PID_sleepdiary_yyyymmdd.csv | Daily in the morning  |  |  |  |
| continuous/wearlog | PID_wearlog_yyyymmdd.csv | Any time participant had removed or started wearing the light logger |  |  |  |
| continuous/wellbeingdiary | PID_wellebeingdiary_yyyymmdd.csv | Daily in the evening |  |  |  |
| demographics | PID_demog_yyyymmdd.csv | Screening questionnaire containing demographic and health information. Completed online before study intake.  |  |  |  |
| discharge/ | PID_ASE_yyyymmdd.csv | Completed at discharge (Monday, day 8).  |  |  | From PID 221 to 231, the discharge folder contains only one csv file names “PID_discharge_yyyymmdd.csv” where all the five questionnaires are saved together. |
| discharge/ | PID_LEBA_yyyymmdd.csv | Completed at discharge (Monday, day 8).  |  |  |  |
| discharge/ | PID_VLSQ8_yyyymmdd.csv | Completed at discharge (Monday, day 8).  |  |  |  |
| discharge/ | PID_feedback_yyyymmdd.csv | Completed at discharge (Monday, day 8).  |  |  |  |
| discharge/ | PID_mTFA_yyyymmdd.csv | Completed at discharge (Monday, day 8).  |  |  |  |


|**Read-out** |**Measurement modality** |**Sampling frequency** |**Timing of sampling** |**N per participant**|
| - | :- | - | - | - |
|**Objective individual light exposure** |Light logger |Continuous measurement  over 7 days |Every 10 seconds  |Approx. 10080 |
|**Objective activity/rest** |Actimeter|Continuous measurement  over 7 days |Every 10 seconds |Approx. 10080 |
|**Chronotype** |Munich  Chronotype Questionnaire (MCTQ,  circadian time)  and  Morning Evening Questionnaire (MEQ,  circadian preference) |1  measurement over 7 days |First  experimental day |1 |
|**Subjective sleep** |Consensus  Sleep Diary (CSD) |7  measurements over 7 days |Every morning |7 |
|**Subjective hourly light exposure and activities** |Modified  Harvard Light  Exposure Questionnaire (modified H-LEA) |7  measurements over 7 days |Every evening |7 |
|**Subjective wellbeing** |WHO-5  wellbeing index (WHO-5) |7  measurements over 7 days |Every evening |7 |
|**Exercise frequency and type** |Exercise log |7  measurements over 7 days |Every evening |7 |
|**Subjective light exposure** |Modified  Harvard Light  Exposure Questionnaire (modified  H-LEA). Experience |24  measurements over 7 days |4 times/day |22 |
||sampling:  punctual measurement  on participants’  current light conditions ||||
| :- | - | :- | :- | :- |
|**Subjective alertness** |Karolinska Sleepiness  Scale (KSS).  Experience sampling:  punctual measurement  on participants'  current light conditions |22  measurements over 7 days |4 times/day |22 |
|**Subjective mood** |MoodZoom questionnaire |22  measurements over 7 days |4 times/day |22 |
|**Experience log** |Custom-made questionnaire  and open-ended questions  about positive and negative experiences wearing  the  light logger |Continuous measurement  over 7 days |Throughout  the experiment |Depending  on participant |
|**Wear log** |Custom-made questionnaire  about time  of  taking  the device  off  and putting it back on |Continuous measurement  over 7 days |Throughout  the experiment |Depending  on participant |
|**Subjective light sensitivity**|Visual Light Sensitivity Questionnaire  8 (VLSQ-8) |1  measurement over 7 days |Last  experimental day |1 |
|**User experience of wearing the light logger** |Open-ended questions |1  measurement over 7 days |Last  experimental day |1 |
|**Sleep environment** |Assessment  of sleep  environment |1  measurement over 7 days |Last  experimental day |1 |
||questionnaire (ASE) ||||
|**Subjective light exposure** |Light  Exposure Behaviour Assessment (LEBA) |1  measurement over 7 days |Last  experimental day |1 |
