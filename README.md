# Sanskrit Heritage Segmenter's Analysis of DCS sentences

Digital Corpus of Sanskrit([DCS](http://www.sanskrit-linguistics.org/dcs/)) is a corpus of more than 600,000 annotated Sanskrit sentences taken from around 250 texts. Sanskrit Heritage Segmenter([SH](http://www.sanskrit.inria.fr)) produces all the possible segments of a given sentence along with all the possible lexical and morphological analyses of each of the segments.

The DCS sentences (extracted from the DCS repository ([DCS-data](https://github.com/OliverHellwig/sanskrit))) are run on the Heritage Segmenter and all the segments with their analyses are extracted and are made available here: [sh_analyses](https://drive.google.com/drive/folders/1-agVobkxVYXw5eIVX2JQHUwzqsR-NTXk?usp=share_link).

## DCS Sentences

1. dcs_sentences.tsv -> All the sentences from DCS (619,906), with their IDs.
2. sentences_recognized.tsv -> Contains only those sentences where all the segments are recognized by the segmenter (474,818).

## Segmenter's Analysis

The analysis of a sentence from the Segmenter is stored in a .tsv format (named with the sentence ID from DCS as ''1.tsv''). Each row/line corresponds to a segment and the fields contain the segment annotations and are described as follows:

1. segment_id
2. word
3. chunk_id
4. pos_in_chunk
5. phase
6. phase_color (phase and phase_color represent the part of speech of the word)
7. stem
8. stem_sense (sense index of the stem in the Heritage dictionary - currently, multiple indices of the same stem are merged together
9. inflectional_morphological_analysis
10. base
11. base_sense
12. derivational_morphological_analysis
13. pre_verb

The sentences, word, stem, base and preverb are encoded in ([WX](https://en.wikipedia.org/wiki/WX_notation)) notation.

(This is a part of the alignment done between the two systems, DCS and SH, to obtain a unified dataset for Word Segmentation and Morphological Parsing in Sanskrit.)