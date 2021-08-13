# tickle.py_precleanser
Two simple python precleanse scripts that generate training examples from a directory for my ASMR generator project

One of them is a directory level wrapper i wrote for an audio chunking script that I found on the prism-samplernn project (https://github.com/rncm-prism/prism-samplernn/blob/master/chunk_audio.py), and the other is the first one that I tried to make by myself that ran into issues when I used it to train my model (zero padding was slightly off by a few samples at the end of each file).

I will say that the prism script is significantly slower than the script that I put together at first, but the prism script is a lot more accurate when it comes to zero padding.

All in all this was a great exercise in learning how to iterate through files at a directory level using python and I learned a lot!

Each script spits out 8 second chunks of 16kHz, 16 bit depth audio from a directory of wav files (chunks that are not 8 seconds in length are zero padded).
For the tickle.py jupyter notebook one you will have to manually create a folder called 'downsampled' in your target directory otherwise the script will not work as intended.
