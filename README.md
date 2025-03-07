                                        # Implementation-of-Honeypot-using-PenTbox-in-Kali-Linux

---

                                                    Information Security IA_1

---

Group members:
Yash Sheth - 16010122310
Minit Shah - 16010122315
Shrusti Vora - 16010122233
Mukul Chaudhari- 16010122311

---

Introduction:
Kali Linux:
A Linux distribution with Debian roots called Kali Linux is made for penetration testing and digital forensics. Offensive Security oversees and provides maintenance for it.Kali Linux offers 600 penetration-testing applications, including Armitage, Nmap, Wireshark, John the Ripper, sqlmap, Aircrack-ing, Burp, and OWASP ZAP.
It was created by Offensive Security employees Mati Aharoni and Devon Kearns through the rewriting of BackTrack, a Linux distribution they had previously used for information security testing and which was based on Knoppix. The Hindu deity Kali served as the name's inspiration.

Honeypot:
Honeypotss are network-attached systems used by hackers to identify and research tactics and types of attacks. Large businesses and cybersecurity-related organisations are the main users, but crooks may use them to hoodwink researchers and disseminate false information.

PenTBox:
PenTBox is a security suite that can be used in penetration testing engagements to perform a variety of activities.Specifically these activities include from cracking hashes,DNS enumeration and stress testing to HTTP directory brute force.

---

--
Stepwise Demonstration:

To set up a honeypot in our Kali Linux system we need to download a tool from GitHub it called Pentbox. This tool is written in ruby language. To download this we use the following command: git clone https://www.github.com/technicaldada/pentbox

![1](/Demonstration-screenshots/1.png)

Then we need to go into the pentbox folder by using cd command as following:
cd pentbox

Here we have a compressed file named pentbox.tar.xz and to extract it, we apply following command:
tar -xzvf pentbox.tar.gz

![2](/Demonstration-screenshots/2.png)

Then we can see a new folder in this directory by using ls command:
ls
Now we go to the pentbox-1.8 directory and check the files using following command:
cd pentbox-1.8 && ls

![3](/Demonstration-screenshots/3.png)

Then we run this ruby tool by using simple command as following:
./pentbox.rb

![4](/Demonstration-screenshots/4.png)

Here we need to go to the Network tools option so type 2 and hit Enter.

![5](/Demonstration-screenshots/5.png)

Yes, now we can see the Honeypot option so we go for it by choosing option 3.

![6](/Demonstration-screenshots/6.png)

Here we can choose 1 for auto configuration this will be fast or we can choose 2 for manual configuration. Manual configuration contains more options but it is for advanced users. For learning we choose the option 1 and hit Enter.

![7](/Demonstration-screenshots/7.png)

Now we can see that we have successfully run honeypot in our localhost on port 80.

![8](/Demonstration-screenshots/8.png)

To check how it works we can go to browser and check our localhost that is 127.0.0.1:80 and then check in the terminal where we started honeypot it will shows the information about him/her who have opened our localhost.

![9](/Demonstration-screenshots/9.png)

![10](/Demonstration-screenshots/10.png)
