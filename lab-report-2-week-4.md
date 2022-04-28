# First changing-file3

`screenshot of code change`
![file3](https://user-images.githubusercontent.com/103155845/164629032-e61e5ff6-97d8-4678-90df-0264987b8396.png)  

[Link to test file 3](https://github.com/wengthree1cm/markdown-parser/blob/main/test-file3.md)  

`screenshot of the symptom output`  
![file3 symptom](https://user-images.githubusercontent.com/103155845/165864084-680c5579-c688-4b0a-ae2f-998d3041ce27.png)


Here we can see that the bug is index out of bound. We know that if indexOf method does not find the thing we required, it will return -1. And we can see that in the file3 there is no "(" ")" which means there is no actual links. Therefore, the indexOf method cannot find "(" so it returns -1.
&nbsp;
&nbsp;

# Second changing-file8

`screenshot of code change`  
![file8 fix](https://user-images.githubusercontent.com/103155845/164643875-ce3fe229-34e0-4464-b6a2-ffd207666634.png)  

[Link to test file 8](https://github.com/wengthree1cm/markdown-parser/blob/main/test-file8.md)  
 

`screenshot of the symptom output`
![file8](https://user-images.githubusercontent.com/103155845/165863844-dbdcbde8-e06e-4533-8ad5-095a1a67bd28.png)  
![file8](https://user-images.githubusercontent.com/103155845/164644005-3438e9f5-4360-44ce-8f11-333574d58903.png) 



When I try to run `java MarkdownParse test-file8.md` in the terminal goes into infinit loop and never stop. I then use Junit test and here we can see that the bug is that it goes into infinit loop. This is because the statement in the while loop is never false, which means that currentIndex is always smaller than markdown.length(). In the file we can see that the file ends with a "[" but not a ")" and that is why the currentindex cannot reach to the markdownlength().
&nbsp;
&nbsp;

# Third changing-file5

`screenshot of code change`
![file5 fix](https://user-images.githubusercontent.com/103155845/164648465-c8028c8e-e659-414b-a2f6-d8ba3093ec03.png)  

[Link to file 5](https://github.com/wengthree1cm/markdown-parser/blob/main/test-file5.md)  

`screenshot of the symptom output`  
![file5 symptom](https://user-images.githubusercontent.com/103155845/165864124-4a7a88ac-8802-44fa-9208-325a49ffe368.png)


In the first picture I added a print statement to see what is in the link and for file5, it prints out "page.com" as a link which is in the bracket. However, this link should not be added as a link because in file 5 we can see that the bracket that contians the link is not closely connected to the Square brackets so that this is not a valid link implementation.








