### BloomFilters
This project aims to test BloomFilters with k-slices.  
Assume we have a giant set of English words,
user enters any string to know if the string is an English word or not.
It is important not to use a dictionary or set because of memory constraints.

#### Usage:
BloomFilters with k-slices:  
1. Clone this repo:  
```
         git clone https://github.com/AbduazizKayumov/BloomFilters.git
```  
2. Install murmur hash and bitstring:
```
         pip3 install mmh3
         pip3 install bitstring
```  
3. Run from command line (note that BloomFilter initialization may take some seconds):
```
         python3 sample_bf.py
```  
4. Enter any string to detect if it is an English word or not.

Optionally, run ```python3 sample_set.py``` (it uses Sets) to compare the memory usage with BloomFilters (both of them displays their own PIDs, find them from memory usage monitoring app in your OS).

Scalable Bloom Filters implementation is in [filters/sbf.py](https://github.com/AbduazizKayumov/BloomFilters/blob/master/filters/sbf.py), run ```python3 sample_sbf.py``` to see how it scales for 370K English words.

English words are from this [project](
https://github.com/dwyl/english-words/blob/master/words_alpha.txt).
