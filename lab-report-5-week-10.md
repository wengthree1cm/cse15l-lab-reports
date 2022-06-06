# lab-report-5

I use `vimdiff` and `bash` to compare two file in the same screen.

The test I used are [487](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/487.html.test) and [517](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/517.html.test)

## test 487 

The expect output is 
![130301654495390_ pic](https://user-images.githubusercontent.com/103155845/172106236-fbdcc10e-2f26-4863-bfda-e5825155d5f5.jpg)
the expect link should be `/my uri` add as a result

After running the vimdiff command I get the result of the following picture
![WechatIMG13027](https://user-images.githubusercontent.com/103155845/172106197-3e703a11-98bc-49c5-97e6-cc76d7b371d3.jpeg)
the left half is my markdown parse, the right half is the given markdownparse

My markdown parse produce the correct result as we can see `/my uri` in the result. The other produce a wrong result 

The bug in the given code should be in this part. Since we see that the result is zero, there might be an error with `openParen` or `closeParen`
which might leads to a wrong `potentiallink`.
<img width="655" alt="截屏2022-06-05 23 32 24" src="https://user-images.githubusercontent.com/103155845/172107883-3ec6acfb-83f0-4043-9653-8af5dd95a396.png">

## test 517

The expect output is 
<img width="1155" alt="截屏2022-06-05 23 28 37" src="https://user-images.githubusercontent.com/103155845/172107303-96dd877f-912f-4cb0-b91b-ae55a10ebe89.png">
The expect link should be `/uri` add as a result. 

after running vimdiff I get the result output.
<img width="1338" alt="截屏2022-06-05 23 27 48" src="https://user-images.githubusercontent.com/103155845/172107212-005e27e5-a318-4819-8943-70e75a068c6d.png">

there is bug in my code, the given code produce a correct result.

this is my code
since we can see my code added `/uri` for two times, means my code does not consider the situation when there are multuple parenthesis.
the bug should be in the while loop, about the `openParen` and `closeParen`.
<img width="769" alt="截屏2022-06-05 23 41 23" src="https://user-images.githubusercontent.com/103155845/172109250-f14755ca-d842-4bc2-858f-55b4b1722e5e.png">
