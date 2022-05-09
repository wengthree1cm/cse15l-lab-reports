# lab-report-3-week-6.md
&nbsp;
&nbsp;
## part1  

I use `~/.ssh/config` to create a file that stores my username and aliais    

![WeChat Screenshot_20220508145822](https://user-images.githubusercontent.com/103155845/167317854-2fa14f42-357d-4062-b9ee-f7ce5fb0b1cc.png)    

Then I login using my alais  
![WeChat Screenshot_20220508150823](https://user-images.githubusercontent.com/103155845/167317862-6c6fad15-871c-418e-9cfb-78595fcaa69d.png)    

Then I copy file "lab-report-1-week-2.md" using `scp` to the server  
![WeChat Screenshot_20220508151007](https://user-images.githubusercontent.com/103155845/167317867-f255a9e7-efdd-43af-9b96-3a2bce6cbd75.png)   
&nbsp;
&nbsp;
## part2  
  
The public key is stored in my github  
![微信截图_20220508155016](https://user-images.githubusercontent.com/103155845/167485901-78e4fe9d-bace-4496-8dfa-555b6ea49bd9.png)   

And this picture is where the private key is stored on my user account   
![微信截图_20220508155051](https://user-images.githubusercontent.com/103155845/167502994-0ca6c9b7-00c3-4364-b829-cc8eee96bf3f.png)
 

I use git commands to commit a new change  
![微信图片_20220509124645](https://user-images.githubusercontent.com/103155845/167486233-8285552f-c143-4f47-971a-0e0617214139.jpg)    

This is the [link](https://github.com/wengthree1cm/markdown-parser/commit/513a660155bb84b8914f449d21e2f16c4fbb57e8) for the resulting commit.   
&nbsp;
&nbsp;
## part3  

I use command `scp -r . ieng6:~/makrdown-parse` to copy the directory to the server.  
These pictures are the successful result of copying.
![微信图片_202205091246451](https://user-images.githubusercontent.com/103155845/167491174-e1a7491b-f43d-498a-ae1e-3775b88d0d88.jpg)
![微信图片_202205091246452](https://user-images.githubusercontent.com/103155845/167491212-a9b6559d-6189-49b6-9ea1-6dfa73a6f2f2.jpg)
![微信图片_202205091246453](https://user-images.githubusercontent.com/103155845/167491225-32c19146-c275-4630-8412-96c2d20ffccf.jpg)  
&nbsp;&nbsp;
Then I login to my server account and use `ls` and found that the `makrdown-parse` is in there  
I then run the test with command `javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java` and `java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest`  and pass the tests

![微信图片_202205091246454](https://user-images.githubusercontent.com/103155845/167491736-86d503ee-0dcf-4625-8b22-00d353de0d53.jpg)

&nbsp;&nbsp;&nbsp;
Finally, I put all the command in one line and successfully copy the whole directory and run the tests in one line. 
![微信图片_20220509132728](https://user-images.githubusercontent.com/103155845/167492085-f965cd6d-44fe-4312-a952-4cf92ae008b7.jpg)
![微信图片_202205091327281](https://user-images.githubusercontent.com/103155845/167492096-0414da6b-fab3-425f-a8aa-eb87795291bc.jpg)







  






