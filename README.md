# MillionSongDataset
This is a scalable computing project done as part of the course work on pyspark

In this assignment we will study a collection of datasets referred to as the Million Song Dataset (MSD),
a project initiated by The Echo Nest and LabROSA. The Echo Nest was a research spin-off from the
MIT Media Lab established with the goal of understanding the audio and textual content of recorded
music, and was acquired by Spotify after 10 years for 50 million Euro.

The main dataset contains the song ID, the track ID, the artist ID, and 51 other fields, such as the
year, title, artist tags, and various audio properties such as loudness, beat, tempo, and time signature.
Note that track ID and song ID are not the same concept - the track ID corresponds to a particular
recording of a song, and there may be multiple (almost identical) tracks for the same song. Tracks are
the fundamental identifier, and are matched to songs. Songs are then matched to artists as well.
The Million Song Dataset also contains other datasets contributed by organisations and the community,

We will focus on the Taste Profile and Top MAGD datasets, but you are free to explore the other datasets
on your own and as part of the challenges. There are many online resources and some publications
exploring these datasets as well.
Taste Profile
The Taste Profile dataset contains real user-song play counts from undisclosed organisations. All songs
have been matched to identifiers in the main million song dataset and can be joined with this dataset to
retrieve additional song attributes. This is an implicit feedback dataset as users interact with songs by
playing them but do not explicitly indicate a preference for the song.
The dataset has an issue with the matching between the Taste Profile tracks and the million song
dataset tracks. Some tracks were matched to the wrong songs, as the user data needed to be matched
to song metadata, not track metadata. Approximately 5,000 tracks are matched to the wrong songs and
approximately 13,000 matches are not verified. This is described in their blog post in detail.
Page 1 of 7Assignment 2 DATA420-20S1 (C)
Audio Features (Vienna University of Technology)
The Music Information Retrieval research group at the Vienna University of Technology downloaded
audio samples for 994,960 songs in the dataset which were available from an online content provider,
most in the form of 30 or 60 second snippets. They used these snippets to extract a multitude of features
to allow comparison between the songs and prediction of song attributes,
Rhythm Patterns
Statistical Spectrum Descriptors
Rhythm Histograms
Temporal Statistical Spectrum Descriptors
Temporal Rhythm Histograms
Modulation Frequency Variance
Marsyas
Timbral features
jMir
Spectral Centroid
Spectral Rolloff Point
Spectral Flux
Compactness
Spectral Variability
Root Mean Square
Zero Crossings
Fraction of Low Energy Windows
Low-level features derivatives
Method of Moments
Area of Moments
Linear Predictive Coding (LPC)
MFCC features
These features are described in detail on the million song dataset benchmarks downloads page and
the audio feature extraction page, and the number of features is listed along with file names and sizes
for the separate audio feature sets.
MSD AllMusic Genre Dataset (MAGD)
Many song annotations have been generated for the MSD by sources such as Last.fm, musiXmatch,
and the Million Song Dataset Benchmarks by Schindler et al. The latter contains song level genre and
style annotations derived from the AllMusic online music guide. We will use the MSD All Music Genre
Dataset (MAGD) provided by the Music Information Retrieval research group at the Vienna University
of Technology.
This dataset is included on the million song dataset benchmarks downloads page and class frequencies
are provided on the MSD AllMusic Genre Dataset (MAGD) details page as well. For more information
about the genres themselves have a look at the AllMusic genres page.
