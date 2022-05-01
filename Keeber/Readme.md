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


### Challenge 6:
![Keeber6](https://user-images.githubusercontent.com/61092858/166133275-6d4f5f56-9a85-4271-9db6-d527099f92ed.png)


### Challenge 7:
![Keeber7](https://user-images.githubusercontent.com/61092858/166133282-89721691-f8b6-43e6-91a3-3fed965b4994.png)


### Challenge 8:
![Keeber8](https://user-images.githubusercontent.com/61092858/166133286-47ea0cdc-0c39-4619-8996-f3c8f944a8fb.png)
