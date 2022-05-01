## An Amazing OSINT Challenge (made by: @matlac#2291, @Gary#4657)

### Challenge 1:
![Keeber1](https://user-images.githubusercontent.com/61092858/166133241-d456b99b-3821-4b42-b78b-e4ce23ef2a5e.png)

### Solution: 
1. Google Search: Keeber Secruity Group and you get the website of the company: keebersecuritygroup.com <img src=https://user-images.githubusercontent.com/61092858/166133575-233c02e7-cc69-4c66-9c27-af9abe18b71c.png height=200 width=700>
2. Do whois search on keebersecuritygroup.com: flag{ef67b2243b195eba43c7dc797b75d75b} ![whois](https://user-images.githubusercontent.com/61092858/166133653-60de22f1-1b92-468e-b1c6-86e79f0ce324.png)

### Challenge 2:
![Keeber2](https://user-images.githubusercontent.com/61092858/166133259-527b594b-cfd0-4bef-957d-98cdef2e29a5.png)

### Solution:
1. Only way to find the past of a website is using web.archive.org and search https:keebersecurity.com
2. look on 19 April snapshots: The team section of the website
3. See the difference of past team and present team: Tiffany Douglas : flag{cddb59d78a6d50905340a62852e315c9}![present team](https://user-images.githubusercontent.com/61092858/166133793-d85cd9c4-205a-40e1-a1c2-96cfbd3c13ea.png)![Past Team](https://user-images.githubusercontent.com/61092858/166133796-d2972921-9f82-40fa-b092-9504e624517b.png)



### Challenge 3:
![Keeber3](https://user-images.githubusercontent.com/61092858/166133263-d991a8e3-d4fc-407e-87b3-3880d184b842.png)

### Solution:
1. From their website we get a github link, let's go their and find all the commits of the Ex Employee![asana secret txt](https://user-images.githubusercontent.com/61092858/166133920-4fd284b0-cb26-4484-9e14-15fe29f80540.png)
2. We get the secret key for asana, go to this github repo: https://github.com/streaak/keyhacks#Asana-Access-Token and see how we can curl to asana users data with the secret key
3. Curl and get the flag: flag{49305a2a9dcc503cb2b1fdeef8a7ac04}![asana flag](https://user-images.githubusercontent.com/61092858/166133987-256201d8-fd1b-4c99-aaad-149fb3abc5e0.png)


### Challenge 4:
![Keeber4](https://user-images.githubusercontent.com/61092858/166133264-c6528aa1-4c76-49cc-8aa7-d50483a19bf7.png)

### Solution:
1. We get the Password Database on this link: https://github.com/keebersecuritygroup/password-manager
2. Download and use john to create hash: keepass2john ksg_passwd_db.kdbx > hash
3. Create wordlist from the github repo: security-evaluation-workflow 
4. Copy all the word from each and every file and paste here: https://design215.com/toolbox/wordlist.php
5. Check the following box remove duplicate words and do not separate hyphenated words
6. Copy the wordlist and use either hashcat or john to crack the password, for hashcat remove the name part![hashcat](https://user-images.githubusercontent.com/61092858/166134350-ff4e4990-9cc0-4b97-b526-ca376b6b1832.jpg)
7. Download Keepass on windows and load the password database and use password: craccurrelss : flag{9a59bc85ebf02d5694d4b517143efba6} ![keepass password](https://user-images.githubusercontent.com/61092858/166134434-10768037-88b8-40a2-a88d-5ef27d656969.png)



### Challenge 5:
![Keeber5](https://user-images.githubusercontent.com/61092858/166133271-8ae81171-859f-41dd-8dfa-1c12db441e71.png)

### Solution:
1. got to know about this article: https://www.nymeria.io/blog/how-to-manually-find-email-addresses-for-github-users
2. then I simply went to check all the commits of the ex employee and added .patch in every commit until I found the flag: flag{2c90416c24a91a9e1eb18168697e8ff5}: ![tiffany email](https://user-images.githubusercontent.com/61092858/166134575-4dbb0aa9-956f-48f9-ab60-001503769a61.png)


### Challenge 6:
![Keeber6](https://user-images.githubusercontent.com/61092858/166133275-6d4f5f56-9a85-4271-9db6-d527099f92ed.png)

### Solution:
1. In previous solution we also got a new email let's pivot it to make use of it:
2. Remove @gmail.com part and think of where this could be used as username, I search for her manually you can use username osint tools like Sherlock and others
3. Found an Instagram account of hers: https://www.instagram.com/tif.hearts.science/
4. Check all her post and you will find one image of a ferry dock which she talks about, in the image if you look closely there is 5 written![279110597_5135446159853761_9027934522620798320_n](https://user-images.githubusercontent.com/61092858/166134751-94bb4037-873f-419e-9ac9-67c04c1e9ce6.jpg)
5. Also Check the github of Tiffany: https://github.com/keeber-tiffany : It says she is from "Maine"
6. Search on Google Maps: ferry dock 5 Portland Maine ![image](https://user-images.githubusercontent.com/61092858/166134936-a6ba0e05-0fab-43c2-9075-c5f9b8dda743.png)
7. Check All the hotels review on yelp, that's a bit frustrating but I guess that's the challenge
8. Residence Inn by Marriott Portland Downtown/Waterfront: Check review of this hotel and sort by newest first, you would get the flag, currently the review is missing

### Challenge 7:
![Keeber7](https://user-images.githubusercontent.com/61092858/166133282-89721691-f8b6-43e6-91a3-3fed965b4994.png)

### Solution:
1. Get the email of hacker: cheerios.fanatic1941@gmail.com
2. let's osint via email: I had solved it using an email osint platform epieos.com but after I solved the hint from there was removed
3. but I got to know the actual solution didn't required it, it require maltego
4. you get that the email is registered on myspace.com
5. create myspcae account and search email of hacker there:![issac anderson](https://user-images.githubusercontent.com/61092858/166135440-2285b66a-a9b8-48d4-8e49-df181ca6fc57.png)
6. flag: flag{4a7e2fcd7f85a315a3914197c8a20f0d}

### Challenge 8:
![Keeber8](https://user-images.githubusercontent.com/61092858/166133286-47ea0cdc-0c39-4619-8996-f3c8f944a8fb.png)

### Solution:
1. Look Closely in the above image, on hackers myspace account you get a new username
2. user sherlock to search this username or use any other username osint tools
3. Pastebin is a place where hacker can post sensitive info: https://pastebin.com/u/cereal_lover1990: visit the link
4. flag: flag{70b5a5d461d8a9c5529a66fa018ba0d0} : ![flag maria data](https://user-images.githubusercontent.com/61092858/166135779-246a17d9-3e29-4cf6-8c2b-3317109283df.png)
