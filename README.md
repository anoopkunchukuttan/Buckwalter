Buckwalter
==========

A small python script that transliterates Arabic text using the Buckwalter Transliteration Scheme. It allows for multiple decisions to be made around whether or not to include all types of diacritics and characters or ignore them. Useful for NLP experiments where you may want to normalize text.

This is adapted from Kenton Murray's script. The functionality is thge same of Kenton's script. The only difference is that the functionality has been wrapped as a class and made available as a Python API (as opposed to commandline in Kenton's script)

Usage of the Python API: 
   ```python 
   import buckwalter as bw
    
   text=u'' 

   # can be a2r [arabic to roman] or r2a [roman to arabic]
   mode='a2r' 
   bw_xlit = bw.Transliterator(mode=mode)
   # constructor supports other arguments as defined in original script
   outtext = bw_xlit.transliterate(text)
   ```


