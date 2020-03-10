# db-jsons-for-good
data files celebrating diversity and lesser-known histories for students

## 20BadassWomen: 
A list of 30 women who were amazing. The bios and quotes come in two languages and were taken from an open source coloring book for teenagers that I co-authored.
List of attributes: 
- id (int); 
- name (str); 
- stem (bool) - determines if a person was stem-related;
- born (int); 
- died (int); 
- bio-pl (str); 
- bio-eng (str); 
- motivational-pl (str); 
- motivational-eng (str);
- pictureUrl (str);


**Gotchas**:
- Gloria Steinem's year of death is null;
- Hatshepsut's years are both negative because BC;

## appNamesAppUsers: 
NOT A JSON: 2 arrays of nouns for a mad lib generator of app ideas;

## climateTeenageActivists: 
A list of 13 teenage climate activists from a few countries. 
List of attributes: 
- id (int); 
- name (str); 
- fromUSA (bool);
- born (int); 
- bio (str); 
- quote (str); 
- twitter (str)


**Gotchas**:
- not all activists have a twitter handle;

## countriesHumanRights
A list of all countries with data on human rights.

## dvdStore-nested-category:
A list of 13 DVDs featuring strong female characters.
List of attributes: 
- id (int); 
- title (str); 
- fromUSA (bool);
- year (int); 
- length (int) -- in minutes;
- director (str); 
- description (str); 
- poster_url (str);
- category (arr):
    - id (int); 
    - name (str);
- discount (bool);
- femaleDirector (bool)


**Gotchas**:
- a nested array;

## dvdStore-simple:
A list of 13 DVDs featuring strong female characters.
List of attributes: 
- id (int); 
- title (str); 
- fromUSA (bool);
- year (int); 
- length (int) -- in minutes;
- director (str); 
- description (str); 
- poster_url (str);
- category (str);
- discount (bool);
- femaleDirector (bool)


**Gotchas**:
- none

## tylerPerryStudios:
Tyler Perry is an American director, screenwriter and producer.
He recently opened Tyler Perry Studios, which are the biggest studios in the USA.
Appart from amazing locations, the studios feature 12 sound stages dedicated to different African-American activists, filmmakers and celebrities.
List of attributes: 
* studios data (array with one object):
    * trivia (str);
    * site (str);
    * overall_size (int) -- in ha;
    * set_size (in) -- in sq feet,
    * owner (object):
        * name (str);
        * bio (str);
        * image
    * sets (array with objects):
        * id (int);
        * description (str);
        * picture_url (str)
    * sound_stages:
        * id (int); 
        * stage_number (int);
    * size (int) -- in sq feet;
    * dedicated (str);
    * bio (str);
    * picture_url (str);

**Gotchas**:
- "studios data" is written with a space;
- there are a few sound stages that are shared by a few people so id is not equal to number as one would think;
- there are a few arrays: trivia, sound stages, locations;
- locations come with an id, description and an image url;

### urbanDict: 
- Ruby and Rails-related version of [urban dictionary](https://www.urbandictionary.com/)
