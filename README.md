# NTU Corpus of Learner English (NTUCLE)


The NTU Corpus of Learner English is a hand-annotated Corpus of Learner English developed in collaboration with the [Language and Communication Centre](https://www.ntu.edu.sg/lcc) at Nanyang Technological University, Singapore. 


The main goal of this corpus was to develop the LCC-NTU English Writing Support System (capable of providing corrective feedback on students' writing), which is now integrated in the [iTELL](https://github.com/lmorgadodacosta/iTELL) suite of applications.

You can read a full description of the corpus, of the new error tag set and annotation process in this 
 [paper](https://aclanthology.org/W17-5901/).


<br> 

The canonical citation for this corpus is:

```
@InProceedings{NTUCLE:2017,
  title = {NTUCLE: Developing a corpus of learner {English} to provide writing support for engineering students},
  author = {Winder, Roger V. P. and MacKinnon, Joe  and Li, Shu Yun  and
Lin, Benedict  and Heah, Carmel  and  Morgado da Costa, Luís and Kuribayashi, Takayuki and Bond, Francis},
  booktitle = {Proceedings of the 4th Workshop on NLP Techniques for Educational Applications (NLPTEA 2017)},
  year = {2017},
  address = {Taipei, Taiwan}
}
```

<br> 

  

**NTUCLE Error Tagset:**

| Error Tag | Description                                                | Category               |
|-----------|------------------------------------------------------------|------------------------|
| ACh       | Wrong choice of article/determiner                         | Articles, determiners  |
| AMiss     | Missing article/determiner                                 | Articles, determiners  |
| AUnn      | Unnecessary article/determiner                             | Articles, determiners  |
| CitForm   | Incorrect citation form                                    | Citations              |
| CitMiss   | Missing citation                                           | Citations              |
| ExpAw     | Awkward expression (meaning is clear)                      | Expression             |
| ExpUC     | Unclear expression (meaning is unclear)                    | Expression             |
| MCase     | Wrong use of upper or lower case                           | Mechanics              |
| MPunc     | Punctuation error                                          | Mechanics              |
| MSpace    | Missing or unnecessary space                               | Mechanics              |
| MSpel     | Spelling error                                             | Mechanics              |
| NCount    | Wrong form of countable/uncountable noun                   | Nouns                  |
| NNum      | Wrong choice of singular/plural form of the noun           | Nouns                  |
| NPoss     | Wrong choice of possessive form                            | Nouns                  |
| PreCh     | Wrong choice of preposition                                | Prepositions           |
| PreMiss   | Missing preposition                                        | Prepositions           |
| PreUnn    | Unnecessary preposition                                    | Prepositions           |
| ProAg     | Pronoun and reference do not agree in number/person/gender | Pronouns               |
| ProCh     | Wrong choice of pronoun                                    | Pronouns               |
| ProMiss   | Missing pronoun                                            | Pronouns               |
| ProRef    | Unclear reference for pronoun                              | Pronouns               |
| ProUnn    | Unnecessary pronoun                                        | Pronouns               |
| SComS     | Comma splice                                               | Sentence structure     |
| SConv     | Convoluted sentence                                        | Sentence structure     |
| SDMod     | Dangling modifier                                          | Sentence structure     |
| SFrag     | Sentence fragment                                          | Sentence structure     |
| SLong     | Overly long sentence                                       | Sentence structure     |
| SMMod     | Misplaced modifier                                         | Sentence structure     |
| SPar      | Parallelism missing                                        | Sentence structure     |
| SRun      | Run-on sentence                                            | Sentence structure     |
| SSub      | Problematic subordinate clause                             | Sentence structure     |
| StyContr  | Contractions                                               | Style                  |
| StyF      | Overly formal words or expressions                         | Style                  |
| StyMood   | Inappropriate use of interrogatives and imperatives        | Style                  |
| StyPron   | Inappropriate use of first and second person pronouns      | Style                  |
| StyWch    | Casual or colloquial words or expressions                  | Style                  |
| SubVA     | Subject and verb do not agree in number and/or person      | Subject-verb agreement |
| TCh       | Wrong choice of link words/phrases                         | Transitions            |
| TMiss     | Missing link words/phrases                                 | Transitions            |
| TUnn      | Unnecessary link words/phrases                             | Transitions            |
| VForm     | Wrong form of the verb                                     | Verbs                  |
| VMiss     | Missing verb                                               | Verbs                  |
| VMod      | Missing, inappropriate or unnecessary modal                | Verbs                  |
| VTense    | Verb tense                                                 | Verbs                  |
| VVoice    | Wrong choice of active or passive voice                    | Verbs                  |
| PosAd     | Wrong position of adjective/adverb                         | Word order             |
| PosW      | Incorrect word order                                       | Word order             |
| WCh       | Wrong choice of word                                       | Words (lexical)        |
| WColloc   | Words do not collocate                                     | Words (lexical)        |
| WForm     | Wrong form of the word                                     | Words (lexical)        |
| WMiss     | Missing words                                              | Words (lexical)        |
| WUnn      | Unnecessary words                                          | Words (lexical)        |
| Oth       | Other errors requiring correction                          | Others                 |