# Corpus Analysis

In-depth analysis of your corpus used to generate this exploratory data analysis is in the `copus_analysis.ipynb` file.

## Corpus statistical properties 

- `Number of words` : 956313
- `Number of types` : 28740
- `TTR` : 0.25
- `Average word length` : 5.7

## Top Words

Top words are extracted by removing stopwords and lowercased:

1. data - 7160
2. experience - 6584
3. work - 5014
4. team - 4987
5. software - 3323
6. security - 3276
7. development - 3125
8. skills - 2825
9. working - 2690
10. learning - 2558
11. business - 2543
12. new - 2284
13. including - 2244
14. role - 2169
15. engineering - 2163
16. years - 2061
17. company - 2057
18. knowledge - 1981
19. design - 1967
20. science - 1943
21. systems - 1876
22. technical - 1841
23. opportunity - 1824
24. support - 1796
25. cloud - 1781

As expected, work and technical words dominate the ranking.

## Statistical properties of LinkedIn corpus to other corpora

### Average word length

![average_word_length](word_length.png)

The `linkedIn` corpus has an average word length much longer than other other corpuses. 
This might be due to long technical words dominating the corpus and maybe to the presence of skills throughout the corpus.

### Type Token Ratio

![ttr](type_token_ratios.png)

The TTR is also high, which can be expected as well, skills related words are repeatedly used throughout the corpus.

### Top words

ratio probabilities is used to identify common words, .

The comparison is made with the `Webtext` and the `treebank` corpus, to get a similarity view.

#### Webtext

```
['film', 'series', 'moments', 'scenes', 'comic', 'actors', 'kevin', 'director', 'roles', 'jackie', 'actor', 'lee', 'scream', 'oscar', 'fans', 'eventually', 'released', 'sequel', 'hilarious', 'ben', 'effective', 'alien', 'decides', 'jim', 'starring', 'sam', 'likely', 'scott', 'effects', 'merely', 'carter', 'played', 'horror', 'allen', 'fi', 'cinematography', 'brief', 'atmosphere', 'subtle', 'supporting', 'humor', 'amusing', 'grace', 'meanwhile', 'audience', 'sean', 'casting', 'trailer', 'detective', 'delivers']
```

The resulting words are skill related words from LinkedIn corpus, but many of them are people's name. 

#### Treebank

```
['plot', 'film', 'don', 'movies', 'character', 'characters', 'audience', 'movie', 'acting', 'guy', 'actor', 'films', 'watching', 'moments', 'looks', 'scenes', 'unfortunately', 'star', 'plays', 'boy', 'tell', 'finds', 'camera', 'directed', 'video', 'entertaining', 'dark', 'story', 'self', 'exactly', 'wife', 'obvious', 'bit', 'guys', 'played', 'scream', 'dialogue', 'happens', 'cast', 'yes', 'god', 'manages', 'whole', 'music', 'emotional', 'sex', 'feature']
```

The top words are skills of different jobs from LinkedIn corpus as well, but they seem to be the sort of word that would be in different context.