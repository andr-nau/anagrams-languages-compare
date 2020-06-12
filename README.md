# anagrams-lang-compare
### This is my training project during attending LinkedIn course "Python: Data Analysis". The project is still in progress.

The initial challenge was to find all anagrams for given English dictionary. I decided to extend this task for different languages and compare the results. 

1. Set of words lists (dictionaries) for different languages (EN, RU, UA, DE, FR) was prepared.

	__German__, __French small__, __English small__ dictionaries were found in open access (http://www.gwicks.net/dictionaries.htm). 

	__English__ bigger size dictionary was provided in LI course (list of words from Webster's Second International Dictionary (1934). The copyright has lapsed, and this file is included in Unix and OS X (and found at /usr/share/dict/words) as a reference wordlist for various uses). 

	__Ukrainian__ dictionary has Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (dict found in https://github.com/brown-uk/dict_uk). 

	__Russian__ dictionaries are from http://www.speakrus.ru/ (free for non-commertial use).


	- RU_small - ~92k words. Nouns, verbs, adjectives, pronouns, prepositions, conjunctions.
	- Ru      - ~124k words. Nouns, verbs, adjectives, pronouns, prepositions, personal/proper names, more compound words. No conjunctions.
	- UA      - ~188k words. Nouns, verbs, adjectives, a lot of compound words. No pronouns, prepositions, conjunctions.
	- EN      - ~230k words. Nouns, verbs, adjectives, pronouns, prepositions, conjunctions, personal/proper names.
	- EN_small - ~194k words. Nouns, verbs, adjectives, pronouns, prepositions, conjunctions, personal names, less proper names.
	- DE      - ~166k words. Nouns, verbs, adjectives, pronouns, prepositions, personal/proper names.
	- FR      - ~336k words.
	- FR_small - ~209k words.

2. Word lists (dictionaries) were divided into sets of words of equal length. To equalize results for different dictionaries sizes (for different languages), I recalculated results in % of overall number of words in dictionary. All languages show similar results in %, so it seems good representation.

	![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/words_percent.png "words in %")

3. Next, actually, - finding of anagrams for different languages. Also using sets of words of equal length. Number of anagrams for each "equal length words" set, absolute values:

	![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/anagrams.png "anagrams")

	And number of anagrams for each "equal length words" set, recalculated in % of length of each set:

	![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/anagrams_percent.png "anagrams in %")

