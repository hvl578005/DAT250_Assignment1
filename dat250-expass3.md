<h1>DAT250: Software Technology Experiment Assignment 3</h1>
<h2>Installation and Verification</h2>
First I did the <i>Verify Integrity of MongoDB Packages</i> tutorial. It went fine and had little to no complaints. I used the PGP/GPG key to check the validation of the MongoDB package. However when I did step 4 <i>Verify the MongoDB installation file</i> I got the right response which is (I copied these from the tutorial because I got the same message, only some numebrs switched out)
<br><br><i>gpg: Signature made Wed Jun  5 03:17:20 2019 EDT
<br>gpg:                using RSA key 4B7C549A058F8B6B
<br<gpg: Good signature from "MongoDB 5.0 Release Signing Key <packaging@mongodb.com>" [unknown]</i>
<br><br>But I also got the following message: 
 <br><br><i>gpg: WARNING: This key is not certified with a trusted signature!
<br>gpg:          There is no indication that the signature belongs to the owner.
<br>Primary key fingerprint: E162 F504 A20C DF15 827F  718D 4B7C 549A 058F 8B6B</i>
 
  <br><br>
 Which got me kind of confused, because the tutorial says if you get that message, you have the package signed but do not currently trust the signing key in your local trustdb. It didnt say how to fix it so I didnt really do anything about it. Sadly I did not take screenshots of it, becauase I didnt see that we had to before the end of the assignment. So when I tried to run the command in terminal again I just got this message
  <br><br><i>gpg: fant ingen gyldig OpenPGP-data.
<br>gpg: klarte ikke å bekrefte signatur.
<br>Husk at signaturfil (.sig eller .asc)
  <br>skal være første filargument på kommandolinja.</i>
<br>Which was kind of annoying because I had already done all of it, and got confirmation the package was signed. And running mongosh on terminal is working so the package is properly installed. To install mongosh I used homebrew.
  
  <h2>Experiment 1: MongoDB CRUD operations</h2>
<h3>Insert</h3>
<img width="627" alt="CRUD1" src="https://user-images.githubusercontent.com/42602758/133826766-47c70253-d571-4e5a-80cd-a87673c04558.png">

<h3>Query</h3>
<img width="624" alt="crud2" src="https://user-images.githubusercontent.com/42602758/133826798-bca58c2e-a608-43c4-930a-1a80a95d5a4c.png">

<h3>Update</h3>
<img width="629" alt="CRUD3" src="https://user-images.githubusercontent.com/42602758/133826832-c28d8a77-81cd-40bf-95ba-7f9cce3f8093.png">
<img width="626" alt="CRUD3_1" src="https://user-images.githubusercontent.com/42602758/133826837-38fe4e7f-9a61-4d43-8c8a-600b2119b5a4.png">

<h3>Remove</h3>
<img width="605" alt="CRUD4" src="https://user-images.githubusercontent.com/42602758/133826882-e7ed94c9-d7cc-409c-a34d-27df5f12c485.png">
<img width="671" alt="crud4_1" src="https://user-images.githubusercontent.com/42602758/133826885-c6a33451-4346-41aa-8457-c03584d7ff42.png">


<h3>Bulk-write</h3>
<img width="1435" alt="CRUD5" src="https://user-images.githubusercontent.com/42602758/133826912-3b99374f-4a1f-4ca0-9354-60b409fd12af.png">




used to start mongosh<br>
brew services start mongodb-community@5.0<br>compass doesnt work on mac? not availebl?
