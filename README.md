# tickle.py_precleanser
A simple python precleanse script to generate training examples from a directory for my ASMR generator project

Spits out 8 second chunks of 16kHz, 16 bit depth audio from a directory of wav files (chunks that are not 8 seconds in length are zero padded).
You will have to manually create a folder called 'downsampled' in your target directory otherwise the script will not work as intended.
