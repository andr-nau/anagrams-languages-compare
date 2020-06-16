# anagrams-lang-compare
## This is my training project during attending LinkedIn course "Python: Data Analysis". The project is still in progress.

The initial challenge was to find all anagrams for given English dictionary. I decided to extend this task for different languages and compare the results. 

__1. Set of words lists (dictionaries) for different languages (EN, RU, UA, DE, FR) has been prepared.__

English main dictionary was provided in LinkedIn course (This is list of words from Webster's Second International Dictionary (1934). 
The copyright has lapsed, and this file is included in Unix and OS X (and found at /usr/share/dict/words) as a reference wordlist for various uses). 

Russian dictionaries are from http://www.speakrus.ru/ (free for non-commercial use).

Ukrainian dictionary found in https://github.com/brown-uk/dict_uk and has Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. 

German, French small, and English small dictionaries were found in open access (http://www.gwicks.net/dictionaries.htm). 


| language | words | nouns | verbs | adjectives | pronouns | prepositions | conjunctions | personal names | proper names | other |
|:---|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|EN		|320k|x|x|x|x|x|x|x|x|
|EN small|194k|x|x|x|x|x|x|x|few|
|UA		|188k|x|x|x||||||many compound words|
|RU		|124k|x|x|x|x|x|x|x|x|compound words|
|RU small|92k|x|x|x|x|x|x|||compound words|
|DE		|166k|x|x|x|x|x|x|x|x|
|FR		|207k|x|x|x|x|x|x|x|x|


__2. All Word lists (dictionaries) has been divided into sets of words of equal length.__ 

To equalize results for different dictionaries sizes (for different languages), I recalculated results in % of overall number of words in dictionary. 
All languages show similar results in %, so it seems good representation.

	![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/words_percent.png "words in %")

__3. Main step - finding of anagrams for different languages.__ 

Anagrams also divided by sets of words of equal length. Next Figure shows number of anagrams for each "equal length words" set (in absolute values):

	![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/anagrams.png "anagrams")

Next picture presents number of anagrams for each "equal length words" set, but recalculated in % of length of each set:

	![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/anagrams_percent.png "anagrams in %")

__Preliminary results:__

- All Slavic languages (RU, UA) have similar number of anagrams.
- German group (EN, DE): German shows results similar to Slavic group, whereas English is very similar by anagrams to French (Romance languages).
- Romance group (FR): French is very similar to English. 
- Questions: why smaller English dictionary has larger number of anagrams, even in "%" representation? 

For Russian it's seems OK: in absolute values, small and big dictionaries has almost equal number of anagrams. In % representation small dictionary shows bigger values - 
to get % scale, we divide almost equal number of anagrams for both dicts for each word length, by different number of words of this length.
Bigger dictionary has bigger number of words of each length, and consequently, smaller % of anagrams. 