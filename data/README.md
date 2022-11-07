## VAD-V-ADJ-filtered.txt: 

To formalize sentiment concepts, we employ the NRC Valence, Arousal, and Dominance (NRCVAD) lexicon (Mohammad, 2018), which provides
manually annotated real-valued scores of valence, arousal, and dominance for 20,000 English words. We use the valence scores and convert them into the range from -1 (the most negative) to 1 (the most
positive). We automatically select single words from the lexicon that are predominantly used as adjectives in the British National Corpus (BNC)5
and sort them in decreasing order by their frequency in the BNC. The N most frequent adjectives that can be used to describe humans or groups of humans
are manually selected as the sentiment words to define the sentiment concepts. The sentiment range [-1, 1] is divided into five intervals: very negative [-1, -0.75], negative (-0.75, -0.25), neutral [-0.25,
0.25], positive (0.25, 0.75), and very positive [0.75,1]. For each interval, N = 100 adjectives are selected.6 These sets of adjectives are then used to
populate the sentence templates to define the sentiment concepts as described in Section 5.


## random_stopwords_tweets.txt:

Acollection of raw tweets collected with stop words. As shown in [Sensitivity_2_sentiment.ipynb](https://github.com/IsarNejad/Procedural-Fairness-Sentiment/blob/main/Sensitivity_2_sentiment.ipynb) 
we use the random tweets as 1) input examples of the classifier in the TCAV procedure 2) concept examples for non-coherent control concepts. 
