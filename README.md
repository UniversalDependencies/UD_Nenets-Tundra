# Summary

The Tundra Nenets UD treebank is converted from the [Tundra Nenets mSUD treebank](https://github.com/surfacesyntacticud/mSUD_Nenets-Tundra). The conversion from mSUD to UD is performed automatically followed by a comprehensive manual revision to ensure compliance with the UD annotation standards.

# Introduction

The treebank currently comprises 171 manually annotated sentences (approximately 11 minutes of recorded speech). The data were collected during a fieldwork session conducted in Moscow in 2017 with a native speaker of Tundra Nenets (Yamal dialect). The session elicited semi-spontaneous speech through visual stimulus–based tasks, including a modified version of the [HCRC Map Task] (https://groups.inf.ed.ac.uk/maptask/maptasknxt.html) and the the so-called Pear Story narrative task (Chafe, 1980).

The spoken data were transcribed by the native speaker using standard Tundra Nenets orthography rather than phonetic or IPA-based notation. Sentence segmentation builds on the original transcription and follows a combined prosodic and semantic approach, in which intonational boundaries are treated as sentence boundaries only when they correspond to semantically complete units; otherwise, adjacent material is merged. The recordings were manually time-aligned at both sentence and lexeme levels in Praat to support morphological and syntactic analysis. The transcription reflects normalized forms and does not capture phonetic variation or morphophonological processes (e.g. sandhi), although the audio data are available for reference.

Annotation focuses on spoken-language phenomena relevant to word-level analysis, especially word boundary identification. An inductive approach was adopted, identifying recurrent phenomena in the data and assigning dedicated tags, informed by spoken UD practices and adapted to the typological properties of Tundra Nenets. The dataset consists mainly of narrative monologues and lacks interactional features such as overlap. Spoken phenomena are divided into non-lexical items (e.g. noises, pauses, hesitation markers), assigned discourse relations, and lexical disruptions (e.g. unfinished words, false starts, repetitions), which affect syntactic structure; pauses are treated either as punctuation or discourse elements depending on function.

Lemmatization preserves dialectal variation due to the absence of a unified written standard. Only inflectional morphology is segmented from stems, while derivational morphology is retained; inflectional suffixes remain in their surface forms, and linking vowels are treated as part of the stem. POS tagging and morphological analysis were performed manually, with inflectional features segmented and glossed following established descriptive traditions and a tagset based on the Leipzig Glossing Rules, adapted to Tundra Nenets.

To account for its complex morphology and syntactic encoding, annotation is based on the morphologically enhanced Surface-Syntactic Universal Dependencies (mSUD) framework (Guillaume et al., 2024). Within the UniDive COST Action (CA21167), UD is extended with a layer for Information Structure roles (e.g. topic and focus). In Tundra Nenets, topicality is reflected in agreement: when a verb agrees with a topical object, the object is annotated as ISRole=Top and the corresponding verbal agreement as ISMarker[Top]=Agr.

The original Cyrillic transcription was transliterated into Latin script, taking into account language-specific properties. Conversion from mSUD to UD is performed in two stages, first from mSUD to SUD and then from SUD to UD, using iteratively applied Grew (Guillaume, 2021) rules.

This treebank is described in detail in Mus et al. (2025), where further information on annotation decisions and linguistic analysis can be found.

# Acknowledgments

The development of this treebank was supported by two research projects: Autogramm: Induction of Descriptive Grammar from Annotated Corpora (ANR-21-CE38-0017), and ThEA: Theoretical and Experimental Approaches to Dialectal Variation and Contact-Induced Change – A Case Study of Tundra Nenets (NKFIH FK 129235). These projects contributed to both the data collection and the creation of the treebank. In addition, this work was supported by COST Action CA21167 —Universality, diversity and idiosyncrasy in language technology ([UniDive](https://unidive.lisn.upsaclay.fr/)).

## References
Chafe, Wallace L. (ed.) 1980. _The pear stories: Cognitive, cultural, and linguistic aspects of narrative production. Advances in Discourse Processes_, vol. III. Ablex, Norwood, NJ, USA.

Guillaume, Bruno. 2021. Graph matching and graph rewriting: GREW tools for corpus exploration, maintenance and conversion. In _Proceedings of the 16th Conference of the European Chapter of the Association for Computational Linguistics: System Demonstrations_, pp. 168–175, Online. Association for Computational Linguistics.

Guillaume, Bruno, Gerdes, Kim, Guiller, Kirian, Kahane, Sylvain and Li, Yixuan. 2024. Joint annotation of morphology and syntax in dependency treebanks. In _Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation_ (LREC-COLING 2024), pp. 9568–9577, Torino, Italia. ELRA and ICCL.

Mus, Nikolett, Guillaume, Bruno, Kahane, Sylvain and Zeman, Daniel. 2025. Creating a multi-layer Treebank for Tundra Nenets. In _Proceedings of the 10th International Workshop on Computational Linguistics for Uralic Languages_, pp. 77-86. 2025.


# Changelog

* 2025-11-15 v2.17
  * Added text of the Pear Story.
* 2025-05-15 v2.16
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.16
License: CC BY-SA 4.0
Includes text: yes
Parallel: no
Genre: spoken
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Bona, Morgane; Guillaume, Bruno; Kahane, Sylvain; Miletić, Aleksandra; Mus, Nikolett; Zeman, Daniel
Contributing: here
Contact: mus.nikolett@gmail.com
===============================================================================
</pre>
