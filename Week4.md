# CSE 15L Week4 - DEBUG

## 1

![test1_change](images/Week4/1st change.png)

The file I tested in [test1](https://github.com/xiaoxia-xia/markdown-parse/blob/main/test1.md), https://github.com/xiaoxia-xia/markdown-parse/blob/main/test1.md

infinite loop: The original one doesn't consider existence of the word after link, so that program keep reading the String after last "("

![test1_Error](images/Week4/1st output.png)

Description: Adding the break law that if meet the last ")", then quit the while loop. The word after ")" will be ignored.


## 2 

![test2_change](images/Week4/2nd change.png)

The file I tested in [test2](https://github.com/xiaoxia-xia/markdown-parse/blob/main/test2.md), https://github.com/xiaoxia-xia/markdown-parse/blob/main/test2.md

outOfIndex exception: Since program will detect the [] then search (), but some time is lack of link in the file

![test2_Error](images/Week4/2nd output.png)

Description: Add the try and catch in case of the exception. If the exception caught, tell the user that "can not detect the link in the file"


## 3

![test3_change](images/Week4/3rd change.png)

The file I tested in [test3](https://github.com/xiaoxia-xia/markdown-parse/blob/main/test3.md), https://github.com/xiaoxia-xia/markdown-parse/blob/main/test3.md

If () leave the blank, the array will not keep anything, neither tell the user leaves the blank place

![test_Error](images/Week4/3rd output.png)

Description: the link is expected to caught in paren. if the thing inside is blank, I leave the note "the paren leaves blank".  