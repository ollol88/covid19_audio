# covid19_audio
We extracted audio files from subjects tested for COVID-19 on the web. We want this to be the first step to provide the machine learning community enough training to develop an algorithm to pre-screen potential cases of COVID-19. 

Leveraging microphones already available on a common smartphone could help in pre-screening who is to be tested and who not, several times a day, remotely. This would massively optimize testing operations.

https://drive.google.com/open?id=1Bp9IPmj1UlEGshYVTWeGUB-01nz6fh0E

# DATA
## Structure of the database
--POSITIVE folder      -> audio of patients tested as positive to COVID-19

--NEGATIVE folder     ->audio of patients tested as negative to COVID-19

--CONTROL               ->audio selected as controls. old audio files (pre covid-19). built 
                                       keeping into consideration characteristics of the speaker and the 
                                       audio quality.

--LINKS file                 ->references to the original videos from which the audio have been  
                                       taken.
## Audio files

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




