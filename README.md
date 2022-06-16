# NTU Corpus of Learner English (NTUCLE)


The NTU Corpus of Learner English is a hand-annotated Corpus of Learner English developed in collaboration with the [Language and Communication Centre](https://www.ntu.edu.sg/lcc) at Nanyang Technological University, Singapore. 


The main goal of this corpus was to develop the LCC-NTU English Writing Support System (capable of providing corrective feedback on students' writing), which is now integrated in the [iTELL](https://github.com/lmorgadodacosta/iTELL) suite of applications.

The corpus contains 180 documents hand-tagged by professional English lecturers. One third (60) of the documents were tagged by two lecturers. Documents that were annotated by two people had their error tags harmonized/adjudicated. A list of documents and whether they have been double annotated can be found in the file [annot_doc.tsv](annot_doc.tsv).


You can read a full description of the corpus, of the new error tag set and of its annotation process in our 
 [paper](https://aclanthology.org/W17-5901/).


This corpus (along with all its annotations) is released under a [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).


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



<br>

The corpus is provided in a simple XML schema. The corpus is organized in three main layers: documents, sentences and words. Errors are SubElements of sentences but are explicitely linked to any number of words in that sentence. A mapping to the full description of error labels is provided above (and in even greater detail in the reference [paper](https://aclanthology.org/W17-5901/)). Here is a simple example:

```
<Corpus corpusID="ntucle-h" title="NTU Corpus of Learner English (Human Annotation)" language="eng"> 
  <Document docID="d0" comment="orig_docid:1">

    (...)

    <Sentence sid="d0s20" sent="The most important benefit of using these advanced curtains is the energy savings that it would provide." comment="origSID/PID=21">
      <Word wid="d0s20w0" sform="The" lemma="the" pos="DT"/>
      <Word wid="d0s20w1" sform="most" lemma="most" pos="RBS"/>
      <Word wid="d0s20w2" sform="important" lemma="important" pos="JJ"/>
      <Word wid="d0s20w3" sform="benefit" lemma="benefit" pos="NN"/>
      <Word wid="d0s20w4" sform="of" lemma="of" pos="IN"/>
      <Word wid="d0s20w5" sform="using" lemma="use" pos="VBG"/>
      <Word wid="d0s20w6" sform="these" lemma="these" pos="DT"/>
      <Word wid="d0s20w7" sform="advanced" lemma="advanced" pos="JJ"/>
      <Word wid="d0s20w8" sform="curtains" lemma="curtain" pos="NNS"/>
      <Word wid="d0s20w9" sform="is" lemma="be" pos="VBZ"/>
      <Word wid="d0s20w10" sform="the" lemma="the" pos="DT"/>
      <Word wid="d0s20w11" sform="energy" lemma="energy" pos="NN"/>
      <Word wid="d0s20w12" sform="savings" lemma="savings" pos="NNS"/>
      <Word wid="d0s20w13" sform="that" lemma="that" pos="IN"/>
      <Word wid="d0s20w14" sform="it" lemma="it" pos="PRP"/>
      <Word wid="d0s20w15" sform="would" lemma="would" pos="MD"/>
      <Word wid="d0s20w16" sform="provide" lemma="provide" pos="VB"/>
      <Word wid="d0s20w17" sform="." lemma="." pos="."/>
      <Error eid="d0s20e0" label="ProAgr" wids="d0s20w6, d0s20w7, d0s20w8, d0s20w14" user="annot_6"/>
    </Sentence>

    (...)

  </Document>

    (...)

</Corpus>
```