# covid19_audio

This is a collection of soundtracks extracted from videos available on the web. It unites short fragments of speech attributed either to subjects tested positive for COVID-19 or random people considered healthy. 

The data is intended to provide ML and AI communities with the first training set to be used in developing algorithms based on sound data for pre-screening of potential COVID-19 cases.

We hope this is to be the first step that will permit us to proof that sounds produced by humans can be enough to discriminate between healthy and unhealthy cases. Success of this step will allow to attract enough interest and attention and consequently collect more targeted data of a better quality.

We hypothesize that easy-anonymizable sounds of human breath and fake cough can be sufficient for high accuracy detection of respiratory problems indicative of flu-like infections, including COVID-19. Moreover, the data collection once established will be effortless since microphones and sound recording apps already available on common smartphone will be sufficient data collection.


https://drive.google.com/open?id=1Bp9IPmj1UlEGshYVTWeGUB-01nz6fh0E

# DATA
## Structure of the database
--POSITIVE folder      -> audio of patients tested as positive to COVID-19

--NEGATIVE folder     ->audio of patients tested as negative to COVID-19

--CONTROL               ->audio selected as controls. old audio files (pre covid-19). built 
                                       keeping into consideration characteristics of the speaker and the 
                                       audio quality.

--LINKS file                 ->references to the original videos from which the audio has been extracted.

## Structure of audio files name

In order:

unique id for the audio

f/m -> gender

age group -> 0: 0-20, 1: 20-40, 2: 40-60, 3: 60+

reference -> if one person is recorded in multiple audio

country of origin (prefix)

language of the audio

result to covid-19 test: 0: negative, 1: positive

severity -> 0 → if negative to covid-19; 1→ positive without symptoms, 2 → positive with    
               symptoms (not hospitalized), 3→ in the hospital or require hospitalization,
               9 → we don’t have information about the severity of the disease

### example: 
    1_f_1_0_1_eng_1_1.wav

this is the first video -> id=1

gender -> f: female

age group -> 20-40

reference -> 0: this is the first audio of that person

country of origin -> 1: USA

language -> eng english

result to codid test: 1 -> positive

severity -> positive without symptoms

### Legend:
language: eng=english, ru: russian, deu: german, chi: chinese, esp: spanish, ita: italian.
country of origing: 1:USA, 11:canada, 7: russia, 49: germany, 86: china, 52: mexico, 34: spain, 57: colombia, 54: argentina, 39: ita




