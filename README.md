# MA Thesis: Language Technology
## Title: "Automatic Annotation of Speech: Exploring Boundaries within Forced Alignment for Swedish and Norwegian"

## Code & Dataset
TBA

## Abstract

In Automatic Speech Recognition, there is an extensive need for time-aligned
data. Manual speech segmentation has been shown to be more laborious than
manual transcription, especially when dealing with tens of hours of speech.
Forced alignment is a technique for matching a signal with its orthographic
transcription with respect to the duration of linguistic units. Most forced
aligners, however, are language-dependent and trained on English data, whereas
under-resourced languages lack the resources to develop an acoustic model
required for an aligner, as well as manually aligned data. An alternative solution
to the training of new models can be cross-language forced alignment, in which
an aligner trained on one language is used for aligning data in another language.
This thesis aimed to evaluate state-of-the-art forced alignment algorithms
available for Swedish and test whether a Swedish model could be applied
for aligning Norwegian. Three approaches for forced aligners were employed:
(1) one forced aligner based on Dynamic Time Warping and text-to-speech
synthesis Aeneas, (2) two forced aligners based on Hidden Markov Models,
namely the Munich AUtomatic Segmentation System (WebMAUS) and the
Montreal Forced Aligner (MFA) and (3) Connectionist Temporal Classification
(CTC) segmentation algorithm with two pre-trained and fine-tuned Wav2Vec2
Swedish models.
First, small speech test sets for Norwegian and Swedish, covering different
types of spontaneousness in the speech, were created and manually aligned to
create gold-standard alignments. Second, the performance of the Swedish dataset
was evaluated with respect to the gold standard. Finally, it was tested whether
Swedish forced aligners could be applied for aligning Norwegian data. The
performance of the aligners was assessed by measuring the difference between
the boundaries set in the gold standard from that of the comparison alignment.
The accuracy was estimated by calculating the proportion of alignments below
a particular threshold proposed in the literature.
It was found that the performance of the CTC segmentation algorithm with
Wav2Vec2 (VoxRex) was superior to other forced alignment systems. The differences
between the alignments of two Wav2Vec2 models suggest that the training
data may have a larger influence on the alignments, than the architecture of the
algorithm. In lower thresholds, the traditional HMM approach outperformed
the deep learning models. Finally, findings from the thesis have demonstrated
promising results for cross-language forced alignment using Swedish models to
align related languages, such as Norwegian.
