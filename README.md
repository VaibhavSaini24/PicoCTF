
This is the solution of the CTF which is based on the Web Explotation
on platform PICOCTF 
- head-dump (Web Exploitation)

--------- CHALLENGE WALKTHROUGH --------------
 1. Start with exploring the web 
 This challenge begin with providing the simple blog website. After instance is launch 
I navigate through the pages , and searching to click on the blog but that can't 
provide any response then  I randomly clicking on the # given on the blogs
that are also not response then I find the hashtags which resopnse and redirect me 
into the other page "#API Documentation.


2. Identifing some critical and point.
 We get the api pages and then we check through sending the api what response
I get but I can't get something critical and then I go for the description 
of the ctf and find some thing headdump then at the end of api pages saw a
section for the headdump and send the request and from there a file is downloades
with extension of ".heapsnapshots"


3. Find the flag :
 In last we have a file now I search for the flag directly using the cat 
command but it will be very large to find .
So ,I use the command to finf the flag
  
/bash
 cat filename | grep "pico"
\
The in the file I got the flag so, which is given below:



That's for this ctf , Keep learning and Keep Practicing


@Vaibhavsaini24
