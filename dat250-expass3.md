<h1>DAT250: Software Technology Experiment Assignment 3</h1>
<h2>Installation and Verification</h2>
First I did the <i>Verify Integrity of MongoDB Packages</i> tutorial. It went fine and had little to no complaints. I used the PGP/GPG key to check the validation of the MongoDB package. When I did step 4 <i>Verify the MongoDB installation file</i> I got the right response which is (I copied these from the tutorial because I got the same message, only some numbers switched out)
<br><br><i>gpg: Signature made Wed Jun  5 03:17:20 2019 EDT
<br>gpg:                using RSA key 4B7C549A058F8B6B
<br<gpg: Good signature from "MongoDB 5.0 Release Signing Key <packaging@mongodb.com>" [unknown]</i>
<br><br>However,  also got the following message: 
 <br><br><i>gpg: WARNING: This key is not certified with a trusted signature!
<br>gpg:          There is no indication that the signature belongs to the owner.
<br>Primary key fingerprint: E162 F504 A20C DF15 827F  718D 4B7C 549A 058F 8B6B</i>
 
  <br><br>
 Which got me kind of confused, because the tutorial says if you get that message, you have the package signed but do not currently trust the signing key in your local trustdb. It didnt say how to fix it so I didnt really do anything about it. Sadly I did not take screenshots of it, becauase I didnt see that we had to before the end of the assignment. So when I tried to run the command in terminal again today (five days later after the first time I did) I just got this message
  <br><br><i>gpg: fant ingen gyldig OpenPGP-data.
<br>gpg: klarte ikke å bekrefte signatur.
<br>Husk at signaturfil (.sig eller .asc)
  <br>skal være første filargument på kommandolinja.</i>
<br>Which was kind of annoying because I had already done all of it, and got confirmation the package was signed. And running mongosh on terminal is working so the package is properly installed. To install mongosh I used homebrew.
 <img width="604" alt="mongosh1" src="https://user-images.githubusercontent.com/42602758/133891739-452121c9-c654-4ad3-ac35-492411757779.png">

  
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


 <h2>Experiment 2: Aggregation</h2>
 <h3>Map Reduce and Aggregation</h3>
 <img width="631" alt="CRUD6_4" src="https://user-images.githubusercontent.com/42602758/133891776-606bdb6e-5d44-412a-a2d1-e285d0b98030.png">
 <br><h3>Additional Operation</h3>
 <img width="603" alt="ADDITIONALOPERATION" src="https://user-images.githubusercontent.com/42602758/133891806-62afeb73-b22e-4ae9-8b00-e0bf2584473b.png">
So when using MapReduce for the additional operation, I got a warning. So I changed to aggregation instead. I didnt get those warnings when doing MapReduce first so I was confused for what happened there. The idea behind the function is to get the customer ID and the order date. Then you can see which customers ordered something on a date. The purpose is to maybe see what day of the week customers buy the most!
 <h3>Pending Issues and Final Notes</h3>
 All in all I liked this assignment, the tutorial was descriptive and easy to follow. Pending issues may be that suddenly MapReduce didnt work and I had to swtch to aggregation, which was weird when it worked fine the other day. I did the additional operation two days later than the first assignments so maybe I forgot to type in something. And I have also learned I have to read the entire assignment before starting it. If I had read it all the way through I would have gotten my screenshots of the verification... 
