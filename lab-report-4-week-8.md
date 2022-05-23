# Lab-report-4  

# [Link](https://github.com/NuojinliXu/markdown-parser) to my repository 

## Snippet 1

The expect output is   
![1](https://user-images.githubusercontent.com/103155845/169738502-08d19b3b-ee26-4823-9a01-4defb1cb5b2e.png)  

The picture of the output test is   
![WeChat Screenshot_20220522202600](https://user-images.githubusercontent.com/103155845/169738553-32930acd-4ef7-4855-9318-4047158f70e7.png)  

## Snippet 2

The expect output is 
![2](https://user-images.githubusercontent.com/103155845/169738628-85262a1b-d3e0-4595-a628-179f28cdf864.png)

The picture of the output test is 
![WeChat Screenshot_20220522202811](https://user-images.githubusercontent.com/103155845/169738649-d72ddc76-1d0b-44a5-bda9-88827558d2eb.png)  

## Snippet 3

The expect output is 
![3](https://user-images.githubusercontent.com/103155845/169738677-8b5b9199-698c-47f8-8158-60b64bbac014.png)  

The picture of the output test is 
![WeChat Screenshot_20220522203124](https://user-images.githubusercontent.com/103155845/169738714-97eb5a4d-c803-45e4-b40f-b3b5abee96ce.png)

# [Link](https://github.com/NLChung9/markdown-parser) to my review repository

## Snippet 1

The expect output is 
![1](https://user-images.githubusercontent.com/103155845/169738818-2586fba6-7ff8-4d1a-ad1a-9c414e5c1e1c.png)

The output test is
![11](https://user-images.githubusercontent.com/103155845/169740051-12ac2a32-feb5-44a5-9104-20705a276bfc.png)  

## Snippet 2  

The expect output is 
![2](https://user-images.githubusercontent.com/103155845/169740119-1e66b713-dfb4-495e-9a2a-0e564ca2db9c.png)

The output test is 
![WeChat Screenshot_20220522210453](https://user-images.githubusercontent.com/103155845/169741263-157cdd14-c969-4556-a84f-cc702a412941.png)


## Snippet 3  

The expect output is 
![3](https://user-images.githubusercontent.com/103155845/169740216-debbccb9-b46d-402b-9bb9-d1ddfb0e1bca.png)  

The output test is  
![33](https://user-images.githubusercontent.com/103155845/169740295-2d1f689d-e7bf-4e83-8f1d-1a657a954945.png)  


Question 1:
My file passes snippet 1 but the review file does not. From the output we can see that the result lacks one link.  
Looking into the file, the problem is because one of the link begins with "`[". I need to change the code so that it  
can handle this case. Speciffically, I need the method to start counting when it detects "[".

Question 2:
For Snippet 2, both my file and review file share the same problem since they have the same test output. What I need to change is to consider the case when there are multiple marenthesis in the link address. From the symptom we can see the link is `a.com(())` but the output is `a.com((`. I want the method to stop when it reaches  
to the last parenthesis. 

Question 3:
For my file, from the test output we can see that my method counted in uneccessary space. What I need to change is to not count in the spaces. To do so,
I need to add verify statement to skip all the space when the method detect a space. 

For my review file, from the test output we can see that my method does not counted in the address `https://www.twitter.com` which it should. Looking at 
testfile3, there are some spaces before the link so I think the problem is that when the close parenthesis is not closely connected to the link address,
 my method does not consider it as a address. So I need to change my method so it can handle case when there are spaces between close parenthesis and the link address. 







