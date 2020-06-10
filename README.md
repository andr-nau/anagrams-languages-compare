# anagrams-lang-compare
This is my training project during attending LinkedIn course "Python: Data Analysis". The project is still in progress. Now I'm looking for the best representative dictionaries for German and French landuages.

I found words lists (dictionaries) for different languages (EN, RU, UA, DE, FR):

- RU_small - ~92k words. Nouns, verbs, adjectives, pronouns, prepositions, conjunctions.
- Ru      - ~124k words. Nouns, verbs, adjectives, pronouns, prepositions, personal/proper names, more compound words. No conjunctions.
- UA      - ~188k words. Nouns, verbs, adjectives, a lot of compound words. No pronouns, prepositions, conjunctions.
- EN      - ~230k words. Nouns, verbs, adjectives, pronouns, prepositions, conjunctions, personal/proper names.
- EN_small - ~194k words. Nouns, verbs, adjectives, pronouns, prepositions, conjunctions, personal names, less proper names.


First, I divided lists into sets of words of equal length. To equalize results for different dictionaries sizes (for different languages), I recalculated results in % of overall number of words in dictionary. All languages show similar results in %, so it seems good representation.

![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/words_percent.png "words in %")

Next, actually, - finding of anagrams for different languages. Also using sets of words of equal length. Number of anagrams for each "equal length words" set, absolute values:

![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/anagrams.png "anagrams")

And number of anagrams for each "equal length words" set, recalculated in % of length of each set:

![Output figure](https://github.com/andr-nau/anagrams-lang-compare/blob/master/anagrams_percent.png "anagrams in %")
