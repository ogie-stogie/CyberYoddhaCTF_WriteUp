# CyberYoddha_CTF
[Write Up Link](https://github.com/tbart27/Pea_CTF/blob/main/README.md)

### Team: Bën
Taylor Bart<br>
Kamal Nadesan<br>
Matt Evans<br>
John Tiffany<br>
Ryan Dunn<br>
<br>
For this CTF, we were able to get 27 flags!. I will go over the flags I submitted or worked on for this CTF (disregading the welcome challenge).
<br>
### Misc: Lorem Ipsum
At first I thought maybe there was secret commands in the message when I noticed keywords like sed, however once I executed a diff on their Lorem Ipsum message and the standard message, I was able to see that there was extra letters that spelled out the flag: CYCTF{latiniscool}
### Forensics: Image Viewer
Using http://fotoforensics.com/ I was quickly able to see that the flag was contained in the metadata of the picture. In the "Lens Serial Number" was the flag: CYCTF{h3h3h3_1m@g3_M3t@d@t@_v13w3r_ICU}
### Cryptography: Beware the Ides of March
The title was anobvious reference to Shakespeare's "Jlius Caesar. From there it was simply finding the offset between the first letter of the encrypted message (JFJAM{j@3$@y_j!wo3y}) and seeing what the translation would have to be to arrive at CYCTF. Then you obtained the flag: CYCTF{c@3$@r_c!ph3r}
### Cryptography: Sus
In a collaboration with Ryan, I was able to tell Ryan that I thought it was a hint towards a Vigenerre cipher and in turn he was able to figure out that key was salad. This resulted in the flag: CYCTF{wouldyoulikesomevinegarwiththat}
### Web Exploitation: Look Closely
A trivial challenge where you check the html for the commented flag: CYCTF{1nSp3t_eL3M3nt?}
### Web Exploitation: Disallow
This was another robots.txt exploit that if you follow the links would lead you to the flag: CYCTF{d33r0b0t$_r_sUp3r10r}<br>
With a little humor, they also had the flag as a [link](https://www.youtube.com/watch?v=dQw4w9WgXcQ).
### Web Exploitation: Data Store
Surprisingly enough, I was able to reuse an injection from peaCTF to overide the authorization portal! By inputting `or 1-- -' or 1 or '1"or 1 or"` I was once agin able to get the flag: CYCTF{1l0v3$q1i}
### Password Cracking: secure (i think?)
This one honestly took me too long because I forgot about MD5. Thankfully, Ryan noticed it right away and was able to obtain the flag: securepassword
### Password Cracking: Crack the Zip!
Simply given a password protected zip file. at first I thought maybe changing the extension would be a clever way to beat it, but an even easier method was using https://passwordrecovery.io/ to get the password not2secure. The flag was then in a plaintext file: cyctf{y0u_cr@ck3d_th3_z!p...}
### Trivia
Trivia 2: Who’s operating system was IBM going to buy before MS-DOS? Gary Kildall<br>
Trivia 3: Which company invented the original hadoop software? Yahoo<br>
Trivia 5: What is a social engineering attack in which someone watches someone else enter private information such as a password called? shoulder surfing<br>
Trivia 6: A Hacker infiltrated one of Microsoft's servers and set up malware inside. The malware laid dormant for months, being unnoticed by the server admins. On Thanksgiving Day, the malware was activated, and it crashed all of the servers and the entire network. What is this type of malware called? logic bomb<br>
Trivia 8: What programming language has this logo: [trivia1.png]<br>
haskell (the creator's discord handle was also Haskell#1426)<br>
<br>
### Conclusion
This was by far our team's best and most well rounded CTF of the semester. A lot of refreshers from 365 were in this CTF, a fun trivia section, and reusable web exploits from previous CTFs! With the exception of OSINT, we solved a challenge from every category as a team too! 27 flags may honestly be close to, if not more than the rest of our semester's CTFs combined so it was nice to have a weekend where I felt like we were putting points on the scoreboard. Personally, my side project is working on the web exploits and hopefully over the next semester or two I'll become proficient enough to complete those sections on my own. 
