# First changing-file3

`screenshot of code change`
![file3](https://user-images.githubusercontent.com/103155845/164629032-e61e5ff6-97d8-4678-90df-0264987b8396.png)  

[Link to test file 3](https://github.com/wengthree1cm/markdown-parser/blob/main/test-file3.md)  

`screenshot of the symptom output`  
![symptom](https://user-images.githubusercontent.com/103155845/164631081-41767c5f-6b98-4079-807b-cdfd1320a142.png)

Here we can see that the bug is index out of bound. We know that if indexOf method does not find the thing we required, it will return -1. And we can see that in the file3 there is no "(" ")" which means there is no actual links. Therefore, the indexOf method cannot find "(" so it returns -1.
&nbsp;
&nbsp;

# Second changing-file8

`screenshot of code change`  
![file8 fix](https://user-images.githubusercontent.com/103155845/164643875-ce3fe229-34e0-4464-b6a2-ffd207666634.png)  

[Link to test file 8](https://github.com/wengthree1cm/markdown-parser/blob/main/test-file8.md)  
 

`screenshot of the symptom output`
![file8](https://user-images.githubusercontent.com/103155845/164644005-3438e9f5-4360-44ce-8f11-333574d58903.png)  

Here we can see that the bug is that it goes into infinit loop.This is because the statement in the while loop is never false, which means that currentIndex is always smaller than markdown.length(). In the file we can see that the file ends with a "[" but not a ")" and that is why the currentindex cannot reach to the markdownlength().
&nbsp;
&nbsp;

# Third changing-file5

`screenshot of code change`
![file5 fix](https://user-images.githubusercontent.com/103155845/164648465-c8028c8e-e659-414b-a2f6-d8ba3093ec03.png)  

[Link to file 5](https://github.com/wengthree1cm/markdown-parser/blob/main/test-file5.md)  

`screenshot of the symptom output`  
![sm file 5](https://user-images.githubusercontent.com/103155845/164648534-47dbf371-642a-41a4-80bf-e282dcbaa633.png)
![sympoppp file5](https://user-images.githubusercontent.com/103155845/164648552-a1fb769a-d72d-4846-b3bf-df19bb7b61c1.png)  

In the first picture I added a print statement to see what is in the link and for file5, it prints out "page.com" which is in the bracket. However, this link should not be added as a link because in file 5 we can see that the bracket that contians the link is not closely connected to the Square brackets so that this is not a valid link implementation.








