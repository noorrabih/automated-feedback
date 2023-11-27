================================================================

                  The SAMER Readability Lexicon

                            Release #1
                           23 July 2020

=================================================================
Summary
=================================================================

The SAMER readability lexicon is a large-scale 26,000-lemma leveled
readability lexicon for Modern Standard Arabic. The lexicon was
manually annotated in triplicate by language professionals from three
regions in the Arab world. Details of the creation process and
analysis of the resulting resource are presented in Al Khalil et
al. (2020).

The creation of this resources was done under the New York University
Abu Dhabi (NYUAD) funded Simplification of Arabic Masterpieces for
Extensive Reading (SAMER) project. The purpose of the SAMER project is
to build a corpus of curriculum reading material, formulate a graded
reader scale for the simplification of modern fiction in Arabic
intended for school-age learners, and then use it to guide the
semi-automated simplification of a number of Arabic works of fiction,
a task performed by human simplifiers and facilitated by
state-of-the-art NLP computational tools. A project overview is
presented in Al Khalil et al. (2017).

When citing this resource, please use:

Al Khalil, Muhamed, Nizar Habash, Zhengyang Jiang. A Large-Scale
Leveled Readability Lexicon for Standard Arabic. In Proceedings of the
12th Conference on Language Resources and Evaluation (LREC 2020),
pages 3053-3062 Marseille, 2020.

@inproceedings{al-khalil-etal-2020-large,
    title = "A Large-Scale Leveled Readability Lexicon for Standard {A}rabic",
    author = "Al Khalil, Muhamed and Habash, Nizar and Jiang, Zhengyang",
    booktitle = "Proceedings of The 12th Language Resources and Evaluation Conference",
    year = "2020",
    address = "Marseille, France",
    publisher = "European Language Resources Association",
    url = "https://www.aclweb.org/anthology/2020.lrec-1.373",
    pages = "3053--3062"
    }

=================================================================
Description of Data
=================================================================

The zipped folder "samer-readability-lexicon.zip" has the following
contents:

README.txt  :   This file.

LICENSE.txt :   The license to use this lexicon.

2020.lrec-1.373-Al-Khalil-Habash-Jiang.pdf :
                A paper describing the creation process of this lexicon.

SAMER-Readability-Lexicon.tsv:
                The lexicon file.

=================================================================
Description of Lexicon File
=================================================================

The basic unit of representation of the Arabic words is the lemma#pos.
Lemmas abstract away from inflectional variants of the words; and pos
refers to is the Part-of-Speech.  The choice of the lemma and POS is
based on the extended SAMA morphological analyses (Maamouri et al.,
2010) produced by the MADAMIRA disambiguation system (Pasha et al.,
2014).  We recommend using MADAMIRA or a similar disambiguation system
aligned with the lemma and POS choices it produces for maximum
compatibility.

For more info on Arabic NLP representations, see Habash (2010).

The lexicon file has nine tab-separated columns of information:

(1) Occurrences: the count of lemma#pos occurrences.

(2) Hindawi (5594310): the percentage of the occurrences of a specific
lemma#pos in the Hindawi literature corpus (from
http://www.hindawi.org/).  The number 5,594,310 is the total number of
words used from that corpus. Details are in Al Khalil et al. (2020).

(3) Giga (5594256): the percentage of the occurrences of a specific
lemma#pos in the Gigaword news corpus (Parker et al., 2011).  The
number 5,594,256 is the total number of words used from that
corpus. Details are in Al Khalil et al. (2020).

(4) lemma#pos: Lemma and Part-of-Speech.

(5) Gloss: English glosses of the lemmas. These glosses include some
inflected forms (plurals particularly) for cases of Arabic broken
plural stems.  The English glosses are only intended as additional
information.

(6) Answer1 - Egyptian: Readability reading by the Egyptian annotator.

(7) Answer2 - Syrian: Readability reading by the Syrian annotator.

(8) Answer3 - Saudi Arabian: Readability reading by the Saudi Arabian annotator.

(9) Readability (rounded average): A rounded average of Answers 1, 2, and 3.

Two Example Entries:

First:

5802 87.75% 12.25% حُبّ#noun love;affection 1 1 1 1

This word, meaning "love; affection" appeared 5,802 times in total
between the two corpora. However it was present in the literature
corpus 7 times more than the news corpus.  This basic vocabulary word
got a consistent readability score of 1 from all the annotators.

Second:

6645 5.13% 94.87% وِلايَة#noun state;province#states;provinces 4 3 4 4

This word, meaning "state;province" appeared 6,645 times in total
between the two corpora. However it was present in the news corpus 19
times more than the literature corpus.  This advanced vocabulary word
got a slightly mixed readability score of two 4s and one 3 leading to
a rounded average of 4.

================================================================
Acknowledgments
================================================================

We would like to thank Ramy Eskander and the team of annotators
at Ramitechs for their help in creating this resource.

================================================================
References
================================================================
Al Khalil, Muhamed, Nizar Habash, Zhengyang Jiang. A Large-Scale
Leveled Readability Lexicon for Standard Arabic. In Proceedings of the
12th Conference on Language Resources and Evaluation (LREC 2020),
pages 3053-3062 Marseille, 2020.

Saddiki, Hind, Nizar Habash, Violetta Cavalli-Sforza and Muhamed
Al-Khalil. Feature Optimization for Predicting Readability of Arabic
L1 and L2. In Proceedings of the ACL Workshop on Natural Language
Processing Techniques for Educational Applications, Melbourne,
Australia, 2018.

Al-Khalil, Muhamed, Hind Saddiki, Nizar Habash, and Latifa Alfalasi. A
Leveled Reading Corpus of Modern Standard Arabic. In Proceedings of
the International Conference on Language Resources and Evaluation
(LREC 2018), Miyazaki, Japan, 2018.

Al-Khalil, Mohamed, Nizar Habash and Hind Saddiki. Simplification of
Arabic Masterpieces for Extensive Reading: A Project Overview. In
Proceedings of the International Conference on Arabic Computational
Linguistics, Dubai, UAE, 2017.

Pasha, A., Al-Badrashiny, M., Diab, M., Kholy, A. E., Eskander, R.,
Habash, N., Pooleery, M., Rambow, O., and Roth, R. (2014). Madamira:
A fast, comprehensive tool for morphological analysis and disambiguation
of Arabic. In Proceedings of the Language Resources and Evaluation
Conference (LREC), pages 1094–1101, Reykjavik, Iceland.

Parker, R., Graff, D., Chen, K., Kong, J., and Maeda, K. (2011). Arabic
Gigaword fifth edition ldc2011t11. Philadelphia: Linguistic Data Consortium.

Maamouri, M., Graff, D., Bouziri, B., Krouna, S., Bies, A., and
Kulick, S. (2010). Standard Arabic morphological analyzer (SAMA)
version 3.1. Linguistic Data Consortium, Catalog No.: LDC2010L01.

Habash, Nizar. Introduction to Arabic Natural Language Processing,
Synthesis Lectures on Human Language Technologies, Graeme Hirst,
editor. Morgan & Claypool Publishers.
================================================================
Copyright (c) 2020 New York University Abu Dhabi. All rights reserved.
================================================================
