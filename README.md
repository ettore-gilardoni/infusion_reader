# infusion_reader
infusion_reader is a program to help people interpret a MS direct infusion analysis.

Mass spectrometry is a useful tool for research, not only to analytical chemists, but also to synthetic chemists as aid to interpret the output of a reaction.
Nevertheless, interpretation of the spectra can be challenging and not straight-forward.

The aim of this code is to help researchers to interpret spectra, highlighting on the spectra the peak corresponding at the interested analyte and eventual cluster commonly found in positive and negative ion mode.
This code is not exhaustive (yet) and it doesn't intend to be. This is just an aid to the spectra interpretation.

The code works on txt, tab separated file. The file must have only two columns, intitled X and Y. X reports the m/z value and Y the counts or the relative intensity of the m/z value in the spectra.

The code asks you to type the formula bruta of the interested molecule to calculate the monoisotopic mass.

You can run the search in both positive and negative ion mode, the code will look for your molecule calculating the molecular ion accordingly.

At the end it prints out a table reporting the identified ions and the accuracy from the theoretical molecular ion.
It also prints out a graph of the spectra, highlighting the ion identified.

So far, the code works for low resolution analyzed, although with a small adjustment of the parameters it can also work for high resolution analyzer

In the folder you find a test.txt file that you can use to test the code. The formula bruta to type is: C9H14N4O3
It is a positive ion mode acquisition.
You can play with the accuracy of the run; however the suggested value is 0.5 for the test.txt file.
