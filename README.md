# The Taylor Swift Corpus -- Version 1 

Last updated: June 2025

## Disclaimer 

Taylor Swift owns the rights to her music and lyrics. I don't claim ownership of anything. The intended use for the corpus is linguistic and/or literary research. The CC-BY-NC-SA 4.0 license was chosen to discourage commercial use and redistribution (without attribution) of copyrighted material. 

The lyrics and metadata (as used in the corpus) were made available by the GitHub user sagesolar (https://github.com/sagesolar/Corpus-of-Taylor-Swift). 


## Corpus Size

The corpus comprises 100763 tokens, of which approx. 90376 are words. The corpus contains 232 songs. 


## IMS Open Corpus Workbench

These corpus files assume familiarity with the IMS Open Corpus Workbench and the corpus query language CQP. The corpus workbench can be downloaded here: https://cwb.sourceforge.io/ 


## The VRT-file 

The VRT-file is not needed to use the corpus if the provided corpus files (the files in 'swift' and 'registry') are put in the required directories. The location of the files has to be specified in the registry-file, found in the folder 'registry'. The VRT-File allows for the corpus to be compiled locally from scratch. 

## The XML-file 

The XML-file is not needed to use the corpus. It can be used for POS-tagging and lemmatization to create another VRT-file.  


## POS-tagging and Lemmatization 

The part-of-speech-tagging and lemmatization was conducted with the Python library spaCy. The language model used was en_core_web_trf (release 3.8.0) which can be found here: https://spacy.io/models/en
The lemmatizer uses the Penn Treebank Tagset (https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html). 

In addition, the lemmatization of several verbs with so-called "g-dropping" (e.g. *makin'*, *starin'*, *gettin'*) was adjusted manually, so that they can be found under the corrresponding lemmata (e.g. *make*, *stare* and *get*). 


## Corpus Structure 

Available language data comprise the POS-tags (Penn Treebank), class-tags (less fine-grained categories than POS) and lemma. 

Songs are tagged as ```<song>...</song>```, albums as ```<album>...</album>```. Every line in every song is tagged as ```<s>...</s>```. 

Additional metadata (structural attributes) are ```album_code```, ```album_title```, ```album_year```, ```album_o_year```, ```s_type```, ```song_title```, ```song_number```, ```song_vault``` and ```song_featured```. For more information on the metadata and the possible values that they take, refer to the file '.info' in the folder 'swift'. 

Different albums can not only be differentiated by the full name of the album but also by album codes, composed of three letters. They are as follows: 

  TSW (Taylor Swift)  
  FER (Fearless)  
  SPN (Speak Now)  
  RED (Red)  
  NEN (1989)  
  REP (Reputation)  
  LVR (Lover)  
  FOL (Folklore)  
  EVE (Evermore)  
  MID (Midnights)  
  TPD (The Tortured Poets Department)  
  OTH (Other Songs)

## Selection of songs 

Sagesolar has prevented duplicate counts of the same lyrics by only selecting one version of every song. That means, versions of songs that are pure remixes or special performances have been excluded. In addition, only the versions of songs with additional lyrics (the highest number of lyrics) have been selected, which includes the '10 Minute Version' version of 'All Too Well' on the album 'Red' and
the 'Feat. More Lana Del Rey' version of 'Snow On The Beach' on the album 'Midnights'. 

Also note that, for each album where a Taylor's Version was available, the version owned by Taylor Swift was chosen. 

The album titles are as follows: 

  Red (Taylor's Version)             
  The Tortured Poets Department (The Anthology)      
  1989 (Taylor's Version)                 
  Speak Now (Taylor's Version)      
  Fearless (Taylor's Version)       
  Reputation                         
  Lover                              
  Midnights (The Til Dawn Edition)   
  Evermore                           
  Folklore                           
  Taylor Swift 