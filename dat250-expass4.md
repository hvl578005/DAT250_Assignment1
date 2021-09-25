
<h1>DAT250: Software Technology Experiment Assignment 4</h1>

<h2>Experiment 1: Spark/Java Framework project and Postman</h2>
For this experiment I used the IDE Eclipse. I've used IntelliJ in the other assignments, but for some reason the program wouldn't run in IntelliJ, and I didn't feel like spending lots of time dealing with error messages so I used eclipse instead.
<br>I quickly discovered the Desktop Agent in Postman didn't work with safari so I switched to chrome. This experiment went fine with little complications. Below are screenshots<br><br> <i>The program running in Eclipse</i>
<img width="1389" alt="Screenshot1_DownloadedProject" src="https://user-images.githubusercontent.com/42602758/134312084-b910c648-dba2-4122-9b82-e973f0bc711d.png">
<i>GET request</i>
<img width="1021" alt="Screenshot3_DesktopAgent" src="https://user-images.githubusercontent.com/42602758/134312159-c827535f-6576-4e0d-923e-b901f7adaa2f.png">
<i>PUT request</i>
<img width="1023" alt="Screenshot4" src="https://user-images.githubusercontent.com/42602758/134312177-746abb12-f347-4fe8-8569-a13805d96d36.png">
<br><h2>Experiment 2: REST API for TODO-items</h2>
To create CRUD operations I used the Spark Framework Documentation, https://sparkjava.com/documentation#. I used the Todo class from the tutorial and added an id which automatically incremented by using AtomicLong. In the Main class I made a Hashmap of the Todo items. I used port 555 because for some reason 8080 didnt want to work even though I shut down the last program.
<br><br><i>POST request</i>
<img width="1051" alt="is added" src="https://user-images.githubusercontent.com/42602758/134767855-009f3895-cba7-4d5e-80e4-27cfbf054f6b.png">
Here I added this element.<br>
<br><i>GET request</i>
<img width="1049" alt="get" src="https://user-images.githubusercontent.com/42602758/134767877-7bf1a043-0009-4b1d-a142-a2d1a3c38b73.png">
Here I retrieve all of the elements in the HashMap.<br>
<br><i>DELETE request</i>
<img width="1029" alt="delete" src="https://user-images.githubusercontent.com/42602758/134767889-10afd12b-dbab-4c44-8a72-11b3b6e2b8ac.png">
Here I delete a chosen element<br>
<br><i>GET request after deleting</i>
<img width="1047" alt="get after deletion" src="https://user-images.githubusercontent.com/42602758/134767905-1881b5de-ec3e-4a8b-9dd7-17dfa76164d4.png">
Here I retrieve my elements once again after performign delete operation, proving it works.
<br>
<br>Link for git repo: https://github.com/hvl578005/DAT250_Expr4
