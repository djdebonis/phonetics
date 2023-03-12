# phonetics
Spanish phonetics system

## Spaanish Phonetics and Phonology
Spanish is a language with extraordinarily consistent phonetic and phonological patterns, which respond consistently to the orthography (written form) of the languge. Unlike English, someone who is confident with the systems of the language could be presented with a completely unknown word, yet they would have no problem pronouncing it because these systems are governed by relatively strict rules.

Let's take the example of the English, "-ough." This ending can be seen in words like "cough," "tough," "plough" and "borough." Yet, if you pronounce these four words, all of them have a different sound for the same "-ough" ending. Spanish, on the other hand, might have the word ending "-er," and it will always be pronounced the same, regardless of the word its being used in.

The benefit of these consistent systems is not only ease-of-pronunciation, but also a high degree of predictability. The degree of predictability is so high, in fact, that I felt a few functions with explicit rule-governed systems (i.e. no training) could transcribe simple text into the International Phonetic Alphabet (IPA).

Part of the benefit to a system that transcribes text into IPA is it saves time in phonetics research. As a linguist conducting studies comparing the 'prescriptive' (what is deemed as 'correct') pronunciation against the 'descriptive' (what is actually said by participants), I will often have two sets of IPA, then compare them to see what results. However, if there was a program to develop the prescriptive list for me, it would definitely save me some time and energy, for it can take a long time to type out the little idiosyncracies of IPA. (Ofcourse, a program that does *everything* for me would be more ideal, but I'm taking this one step at a time.)

This code isn't complete yet. Here are the plans:
* (1) create a system that will take a string of a *single* word and return a list of strings, one being the 'prescriptive' transcription, and the others being common, accepted dialectical variations.
  * for example, it might take the string: "playa" and return a list of: [plaʝa], [plaja], [plaʃa], [plaʒa], & [plad͡ʒa].

* (2) upgrade the system so that, instead of just returning the basic allophones, it also returns environment-dependent variations of the allophones.
  * for example, the initial system might return [di̯ente] where as the upgrades system might return [di̯en̪te], signifying the dental-assimilation (dentalization?) of the /n/ due to the /t/ that proceeds it

* (3) upgrade the system yet again so that, instead of just returning individual words, it will also return entire phrases/sentences.
  * (This sounds a lot more straightforward than it is. It is not as simple as iterating over a string split into a list of words, because there are also rules that govern how words 'chain' together, or in other words, how they break into syllables when they are placed next to one another. As a matter of fact, this is likely what causes native English speakers to think of Spanish as sounding 'machine-gun' like.)
  * an example of this would be: "Él y yo fuimos al parque" would become [e-li-ʝo-fu̯i-mo-sal-paɾ-ke]

This will hopefully be the first of a lot of linguistics-based (specifically phonetics & phonology) repos that I develop on here.
