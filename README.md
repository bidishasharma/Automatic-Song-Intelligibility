# Automatic Evaluation of Song Intelligibility using Singing Adapted STOI and Vocal-specific Feature

An objective machine-driven measure of song intelligibility would be of great utility for various music information retrieval tasks. Song intelligibility mostly depends on two factors, the amount of interference caused by background accompaniment, and the quality of singing vocal. We leverage these two factors to determine the intelligibility of a song. For the first factor, we adapt a well known method for intelligibility prediction of noisy speech, short term objective intelligibility (STOI), to singing. The singing-adapted STOI considers the polyphonic song as a time-frequency weighted noisy version of the extracted singing vocal. We use U-net based audio source separation method to extract singing vocal from a polyphonic song. The singing vocal shares the same underlying physiological mechanism for production as that of speech, with some differences in the pronunciation and prosody of the phonemes. Therefore, for the second factor, we have introduced vocal-specific features to measure the intelligibility of the singing vocal, which are excitation source, spectral, and prosodic singing characteristics. We perform detailed analysis on each of these features to establish their efficacy for quantifying song intelligibility. We train a regression model to derive the intelligibility scores using a combination of the vocal-specific features and singing adapted STOI, obtaining a significant improvement in performance. The correlation between the intelligibility score obtained using proposed framework and human-rated intelligibility score is 0.81, which shows the efficacy of the proposed approach.

## Dependencies

1. Matlab2017b
2. libsvm-3.24
3. voicebox
4. Wav-U-Net (https://github.com/f90/Wave-U-Net)

## Instructions

1. SongIntelligibility.tar.gz containes the main program and all dependent functions used in this work.
2. SongIntelligibilityMain.m is the Main Program.
3. Please email to the author (s.bidisha@nus.edu.sg), if you want to use the pretrained SVM model for automatic song intelligibility evaluation.

