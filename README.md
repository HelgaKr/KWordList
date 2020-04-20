# KWordList

KWordList is a small program that can create word lists based on Korean language corpora. 
The program was developed as a part of the Master of Applied Linguistics Thesis by Olga Kriukova (University of Saskatchewan). 
If you want to use your code in your study, you are more than welcome to do so, but please cite this thesis (citation format may be found below),
if you use it for your research.

In this repository, you can find two files: KWordList_source and KWordList_GUI. The first one contains a raw script that was used in my study, and that can be reused with minor changes (directory, criteria values, etc.). The second one is a beta version of the program with GUI (Graphical User Interface) that may be used in Python and do not require any changes to be done in the code by the user. 
An executable file for the second version will appear soon here and on the www.topik-tips.com website.

#Description

1)	KWordList takes a corpus or corpora in .txt format as an input (all your files should be in one directory). 
2)	KWordList deletes all non-Korean symbols from the uploaded corpus to allow accurate word counting.
3)	KWordList tags parts of speech (POS) and lemmatizes all the words in the uploaded corpus. 
Note: For this purpose, the KoNLPy package was used (Park & Cho, 2014). KWordList can tag POS with Mecab, Kkma, and Okt taggers. The taggers detailed description, performance comparison, other useful information may be found on the KoNLPy website https://konlpy.org/en/latest/morph/. Personally, for small size corpora, I would recommend Kkma, for larger corpora – Mecab. 
4)	KWordList excludes the general and/or academic vocabulary from the list of the words that occurred in your corpus. 
Note: In the KWordList interface, you can choose what levels to exclude (Korean Learner’s List (Jo, 2003): Beginner(A), Intermediate(B), Advanced(C), or Academic Vocabulary List (Shin, 2004).
5)	KWordList measures a range of each word. 
Note: In this study, the range is in how many sub-corpora a specific word has occurred. If you use KWordList to build a list for one text file, please set the range value to 0. In other cases, the range depends on the study.
6)	KWordList measures a frequency of the words that have passed the range criteria. 
Note: You can set your frequency criteria. 
7)	KWordList measures dispersion (deviation of proportions or DP (Gries, 2008)). 
Note: This value can show how evenly a word is distributed across sub-corpora. The closer the value to 0, the better is the distribution. The closer the values to 1, the worse is the distribution. You can set your DP criteria, or if you do not need it, just set it to 1 in the program.
8)	KWordList searches for the collocations for the words that passed all the criteria. 
Note: If you do not need collocations, just choose “No” in the interface.
9)	KWordList counts the coverage of your corpus by your list, by Korean Learner’s List(Jo, 2003), and by Korean Academic Vocabulary List (Shin, 2004). 
10)	KWordList gives you a .csv (Comma Separated Values) file output, and if you choose to have statistics, a .csv file with coverage percentages and .txt files with the words that were excluded by Korean Learner’s List and (if required, Academic Vocabulary List).
Note: To open your .csv file, please open a blank notebook in your Microsoft Ofice Excel (or equivalent) first. Then, open “Data” -> From Text/CSV. In opened explorer, choose your .csv location. Then, in opened preview, click on the “File origin” dropdown menu and choose 65001: Unicode (UTF-8). After that, press “Load”. Your results are ready!  

Please note: that some extra features are planned to be added soon.

#References

Bird, S., & Loper, E. (2009). Natural Language Processing with Python. Natural Language Processing with Python. O’Reilly Media Inc.
Gries, S. T. (2008). Dispersions and adjusted frequencies in corpora. International Journal of Corpus Linguistics, 13(4), 403–437.
Jo, N. (2003). Hangugeo hakseubyong eohwi seonjeong gyeolgwa bogoseo [Report on the results of vocabulary selction for learners of Korean]. Seoul: National Institute of Korean Language.
Park, E. L., & Cho, S. (2014). KoNLPy: Korean natural language processing in Python. In Proceedings of the 26th Annual Conference on Human & Cognitive Language Technology. Chuncheon.
Shin, M. (2004). Gugeo sagodogueo gyoyung yeongu [A study on Korean academic vocabulary education]. Seoul National University.


# Citation
Kriukova, O. (2020). Creating a Korean Engineering Academic Vocabulary List (KEAVL): Computational Approach. 
University of Saskatchewan.

