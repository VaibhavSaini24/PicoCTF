
This is the solution of the CTF which is based on the Web Explotation
on platform PICOCTF 
- head-dump (Web Exploitation)

--------- CHALLENGE WALKTHROUGH --------------
 1. Start with exploring the web 
 This challenge begin with providing the simple blog website. After instance is launch 
I navigate through the pages , and searching to click on the blog but that can't 
provide any response then  I randomly clicking on the # given on the blogs
that are also not response then I find the hashtags which resopnse and redirect me 
into  the other page "#API Documentation.

![Screenshot From 2025-07-04 01-44-42](https://github.com/user-attachments/assets/47cf99b8-179d-46ad-afee-c6d4ace981ff)


![Screenshot From 2025-07-04 01-44-57](https://github.com/user-attachments/assets/c84b925a-a86c-4587-b488-8ec473d7a91f)



3. Identifing some critical and point.
 We get the api pages and then we check through sending the api what response
I get but I can't get something critical and then I go for the description 
of the ctf and find some thing headdump then at the end of api pages saw a
section for the headdump and send the request and from there a file is downloades
with extension of ".heapsnapshots"

![Screenshot From 2025-07-04 01-45-12](https://github.com/user-attachments/assets/1100b6bd-3312-466e-955b-b1ad3fe69286)




5. Find the flag :
 In last we have a file now I search for the flag directly using the cat 
command but it will be very large to find .
So ,I use the command to finf the flag
  
/bash
 cat filename | grep "pico"
\
The in the file I got the flag so, which is given below:


![Screenshot From 2025-07-04 01-45-55](https://github.com/user-attachments/assets/8be2af62-8285-47ac-a619-0bf84b3f8ff6)



That's for this ctf , Keep learning and Keep Practicing


@Vaibhavsaini24
