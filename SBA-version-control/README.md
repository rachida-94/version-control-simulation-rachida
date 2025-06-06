SBA version control project:
I created a new repository  on GitHub and then copied the URL. Using clone command, I cloned the repository to my local machine .I named  the repository "SBA-version-control", and  inside this repository I createed an "index.html" file.


first, I created the branch called <feature/header> where I added basic HTML structure along with a header element. After making the changes, I staged and committed the file . When I tried switching back to <main> ,I received an error.Using the git branch command,I found that <feature/header> was the only branch, so I had to create a main branch manually. 


Next , I created another branch called <feature/footer> . In this branch, I added  footer element at the bottom of the HTML file , then staged and committed the changes.After that , I switched back to <feature/header> branch and added the footer element inside the body element,then committed those changes as well. 

Afterward,I switched to the main  branch and merged the <feature/header> into main, followed by  merging <feature/footer>into main. A conflict occurred because both branches had changes involvig the <footer> element.One version had <footer></footer> at the bottom of the HTML file , while the other included <footer>&copy; 2025 My Website</footer> inside the body element.
To resolve the conflict, I kept the version with the copyright footer inside the body and removed the empty oneat the bottom.I then staged and committed the resolved file , used git status  to  ensure everything was correct ,and finally pushed the updated repository to Github . 
To finalize ,I made small change by adding an exclamation mark to the header in my file. This allowed me to create a pull request from main  to review/main .