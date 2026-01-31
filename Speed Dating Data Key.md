# Speed Dating Data Key

Source: `Speed Dating Data Key.doc` (converted to Markdown for reference)
Column names follow `Speed Dating Data.csv` and preserve original spellings (e.g., `positin1`, `undergra`).

## Identifiers
- iid: unique subject number, grouped by wave, id, gender.
- id: subject number within wave.
- gender: Female=0, Male=1.
- idg: subject number within gender, grouped by id and gender.

## Experimental condition and wave
- condtn: 1=limited choice, 2=extensive choice.
- wave: wave number (see table).

### Wave details
| Wave | Date | Preference scale | Variations | # Males | # Females |
| --- | --- | --- | --- | --- | --- |
| 1 | Oct 16, 2002 | 100 pt allocation | - | 10 | 10 |
| 2 | Oct 23, 2002 | 100 pt allocation | - | 16 | 19 |
| 3 | Nov 12, 2002 | 100 pt allocation | - | 10 | 9 |
| 4 | Nov 12, 2002 | 100 pt allocation | - | 18 | 18 |
| 5 | Nov 20, 2002 | 100 pt allocation | undergrads | 10 | 10 |
| 6 | Mar 26, 2003 | 1-10 scale | - | 5 | 5 |
| 7 | Mar 26, 2003 | 1-10 scale | - | 16 | 16 |
| 8 | Apr 2, 2003 | 1-10 scale | - | 10 | 10 |
| 9 | Apr 2, 2003 | 1-10 scale | - | 20 | 20 |
| 10 | Sep 24, 2003 | 100 pt allocation | - | 9 | 9 |
| 11 | Sep 24, 2003 | 100 pt allocation | - | 21 | 21 |
| 12 | Oct 7, 2003 | 100 pt allocation | Budget: only allowed to say yes to 50% of people met | 14 | 15 |
| 13 | Oct 8, 2003 | 100 pt allocation | Different M.C. | 9 | 10 |
| 14 | Oct 8, 2003 | 100 pt allocation | Different M.C. | 18 | 20 |
| 15 | Feb 24, 2004 | 100 pt allocation | - | 19 | 18 |
| 16 | Feb 25, 2004 | 100 pt allocation | - | 8 | 6 |
| 17 | Feb 25, 2004 | 100 pt allocation | - | 14 | 10 |
| 18 | Apr 6, 2004 | 100 pt allocation | brought a magazine | 6 | 6 |
| 19 | Apr 6, 2004 | 100 pt allocation | brought a book | 15 | 16 |
| 20 | Apr 7, 2004 | 100 pt allocation | brought a book | 8 | 6 |
| 21 | Apr 7, 2004 | 100 pt allocation | brought a magazine | 22 | 22 |

## Event/night variables (speed-dating session)
- round: number of people met in wave.
- position: station number where met partner.
- positin1: station number where started.
- order: number of the date that night when met partner.
- partner: partner's id number the night of event.
- pid: partner's iid number.
- match: 1=yes, 0=no.
- int_corr: correlation between participant's and partner's ratings of interests at Time 1.
- samerace: participant and partner same race (1=yes, 0=no).
- age_o: age of partner.
- race_o: race of partner.
- pf_o_att/pf_o_sin/pf_o_int/pf_o_fun/pf_o_amb/pf_o_sha: partner's stated preferences at Time 1 (same 6 attributes as attr1_1).
- dec_o: partner's decision the night of event.
- attr_o/sinc_o/intel_o/fun_o/amb_o/shar_o: partner's ratings of participant (1-10).
- like_o: partner's overall liking (1-10).
- prob_o: partner's estimate that participant will say yes (1-10).
- met_o: partner met participant before (1=yes, 2=no).

## Signup / Time 1 survey
[Survey filled out by students registering for the event.]

### Demographics and background
- age: participant age.
- field: field of study.
- field_cd: field coded:
  - 1=Law
  - 2=Math
  - 3=Social Science, Psychologist
  - 4=Medical Science, Pharmaceuticals, and Bio Tech
  - 5=Engineering
  - 6=English/Creative Writing/Journalism
  - 7=History/Religion/Philosophy
  - 8=Business/Econ/Finance
  - 9=Education, Academia
  - 10=Biological Sciences/Chemistry/Physics
  - 11=Social Work
  - 12=Undergrad/undecided
  - 13=Political Science/International Affairs
  - 14=Film
  - 15=Fine Arts/Arts Administration
  - 16=Languages
  - 17=Architecture
  - 18=Other
- undergra: undergraduate school attended.
- mn_sat: median SAT score of undergraduate institution (Barron's 25th Edition); proxy for intelligence.
- tuition: tuition from Barron's 25th Edition college profiles.
- race:
  - 1=Black/African American
  - 2=European/Caucasian-American
  - 3=Latino/Hispanic American
  - 4=Asian/Pacific Islander/Asian-American
  - 5=Native American
  - 6=Other
- imprace: importance (1-10) that a date be same racial/ethnic background.
- imprelig: importance (1-10) that a date be same religious background.
- from: where originally from (before coming to Columbia).
- zipcode: zip code where participant grew up.
- income: median household income by zip code using Census Bureau lookup `http://venus.census.gov/cdrom/lookup/CMD=LIST/DB=C90STF3B/LEV=ZIP`.
  - Missing income means participant is from abroad or did not enter zip code.

### Goals and habits
- goal: primary goal for participating:
  - 1=Seemed like a fun night out
  - 2=To meet new people
  - 3=To get a date
  - 4=Looking for a serious relationship
  - 5=To say I did it
  - 6=Other
- date: frequency of dates:
  - 1=Several times a week
  - 2=Twice a week
  - 3=Once a week
  - 4=Twice a month
  - 5=Once a month
  - 6=Several times a year
  - 7=Almost never
- go_out: how often participant goes out (not necessarily on dates), same scale as `date`.
- career: intended career.
- career_c: career coded:
  - 1=Lawyer
  - 2=Academic/Research
  - 3=Psychologist
  - 4=Doctor/Medicine
  - 5=Engineer
  - 6=Creative Arts/Entertainment
  - 7=Banking/Consulting/Finance/Marketing/Business/CEO/Entrepreneur/Admin
  - 8=Real Estate
  - 9=International/Humanitarian Affairs
  - 10=Undecided
  - 11=Social Work
  - 12=Speech Pathology
  - 13=Politics
  - 14=Pro sports/Athletics
  - 15=Other
  - 16=Journalism
  - 17=Architecture

### Activity interests (1-10)
- sports: playing sports/athletics
- tvsports: watching sports
- exercise: body building/exercising
- dining: dining out
- museums: museums/galleries
- art: art
- hiking: hiking/camping
- gaming: gaming
- clubbing: dancing/clubbing
- reading: reading
- tv: watching TV
- theater: theater
- movies: movies
- concerts: going to concerts
- music: music
- shopping: shopping
- yoga: yoga/meditation

### Expectations
- exphappy: expected happiness with people met (1-10).
- expnum: expected number (out of 20) interested in dating participant.

## Preference and self-rating scales (Time 1)
Waves 6-9 use a 1-10 scale. Waves 1-5 and 10-21 use 100-point allocations across the 6 attributes (total must equal 100).

Attributes: Attractive, Sincere, Intelligent, Fun, Ambitious, Shared interests/hobbies.

- attr1_1/sinc1_1/intel1_1/fun1_1/amb1_1/shar1_1: importance of attributes in a potential date (self preferences).
- attr4_1/sinc4_1/intel4_1/fun4_1/amb4_1/shar4_1: what you think MOST fellow men/women look for.
- attr2_1/sinc2_1/intel2_1/fun2_1/amb2_1/shar2_1: what you think the opposite sex looks for.
- attr3_1/sinc3_1/intel3_1/fun3_1/amb3_1: self-ratings of own attributes (1-10).
- attr5_1/sinc5_1/intel5_1/fun5_1/amb5_1: how others perceive you (1-10).

## Scorecard (during the event)
[Filled out after each date during the event.]

- dec: decision (1=yes, 0=no).
- attr/sinc/intel/fun/amb/shar: partner attributes (1-10).
- like: overall liking (1-10).
- prob: how probable partner will say yes (1-10).
- met: met partner before (1=yes, 2=no).

## match_es (mid-event)
- match_es: estimated number of matches (mutual yes).

## Halfway through event (mid-event questionnaire)
- attr1_s/sinc1_s/intel1_s/fun1_s/amb1_s/shar1_s: importance of attributes in a potential date (1-10).
- attr3_s/sinc3_s/intel3_s/fun3_s/amb3_s: self-ratings (1-10).

## Follow-up / Time 2 (day after event)
- satis_2: satisfaction with people met (1-10).
- length: 1=Too little, 2=Too much, 3=Just right (4-minute dates).
- numdat_2: 1=Too few, 2=Too many, 3=Just right (number of speed dates).

### Preferences (Time 2)
- attr7_2/sinc7_2/intel7_2/fun7_2/amb7_2/shar7_2: actual importance of attributes in decisions (100-point allocation).
- attr1_2/sinc1_2/intel1_2/fun1_2/amb1_2/shar1_2: importance in a potential date (see Time 1 scale note).
- attr4_2/sinc4_2/intel4_2/fun4_2/amb4_2/shar4_2: what you think MOST fellow men/women look for.
- attr2_2/sinc2_2/intel2_2/fun2_2/amb2_2/shar2_2: what you think the opposite sex looks for.
- attr3_2/sinc3_2/intel3_2/fun3_2/amb3_2: self-ratings (1-10).
- attr5_2/sinc5_2/intel5_2/fun5_2/amb5_2: how others perceive you (1-10).

## Follow-up 2 / Time 3 (3-4 weeks after matches sent)
- you_call: number of matches participant contacted to set up a date.
- them_cal: number of matches who contacted participant.
- date_3: have you been on a date with any matches? (1=Yes, 2=No).
- numdat_3: number of matches participant has gone on a date with so far.
- num_in_3: if yes, how many? (see survey text; often used with numdat_3).

### Preferences (Time 3)
- attr1_3/sinc1_3/intel1_3/fun1_3/amb1_3/shar1_3: importance of attributes in a potential date (1-10).
- attr7_3/sinc7_3/intel7_3/fun7_3/amb7_3/shar7_3: actual importance in decisions (100-point allocation).
- attr4_3/sinc4_3/intel4_3/fun4_3/amb4_3/shar4_3: what you think MOST fellow men/women look for.
- attr2_3/sinc2_3/intel2_3/fun2_3/amb2_3/shar2_3: what you think the opposite sex looks for.
- attr3_3/sinc3_3/intel3_3/fun3_3/amb3_3: self-ratings (1-10).
- attr5_3/sinc5_3/intel5_3/fun5_3/amb5_3: how others perceive you (1-10).
