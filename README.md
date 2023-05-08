Download Link: https://assignmentchef.com/product/solved-si-507-homework-11-flask
<br>
<strong>Homework Objectives</strong>

–   Understand how virtual environments work in python, and know why they are used

–   Be able to install Flask and use Flask to create basic web applications

–   Be able to use templates to integrate python and HTML code to create dynamic web pages




<strong>Helpful Resources</strong>




Readings

<ul>

 <li>Flask Web Development, <a href="https://umich.instructure.com/courses/196493/files/7519744/download?verifier=YgReo9hmJktqtqYTNef7MaeLsVHXZ4TVqD0fdPUu&amp;wrap=1">Chapter 1: Installation</a></li>

 <li>Flask Web Development, <a href="https://umich.instructure.com/courses/196493/files/7519745/download?verifier=1OrVZ2Z2ooBFz3W3KT9tdzOqxwsWLoe8Y7vx8OBo&amp;wrap=1">Chapter 2: Basic Application Structure</a></li>

 <li>Flask Web Development, <a href="https://umich.instructure.com/courses/196493/files/7519746/download?verifier=UF3Bffm4sFlhnGR16R4oUQxquuCprnw8DeTwvIud&amp;wrap=1">Chapter 3: Templates</a></li>

</ul>




Other

<ul>

 <li>org API documentation: <a href="https://newsapi.org/docs">https://newsapi.org/docs</a></li>

</ul>







For this assignment, you will be creating a basic Flask application that greets a user and tells them the top technology news stories for that day.




<strong>Part 1 – Setting Up Flask [6 points]</strong>

<ol>

 <li>Create a directory for your homework assignment.</li>

 <li>Inside that directory, set up a virtual environment called “flask_ve” and, after activating it, install flask and requests modules.</li>

 <li>Create the “requirements.txt” file</li>

 <li>Add the “top_headlines.py” file. You can download the starter version of the file <a href="https://www.dropbox.com/s/qazv1578pu1yelr/top_headlines.py?dl=0">here</a>. You will insert your code into it in part 2.</li>

 <li>Create the “templates” directory.</li>

</ol>




Take a screenshot of your homework directory in Finder/Explorer. Upload it to Canvas as part of your submission. We will be looking to make sure that all the files are in the correct location.




<strong>Part 2 – Greeting the user and showing current technology news [14 points]</strong>

In this part, you will create a web app that greets the user by name and shows her/him the top five current technology news headlines. This content will be displayed by going to the following web page: http://127.0.0.1:5000/newsfor/&lt;user_name&gt;. So, if, for example, one were to go to <a href="http://127.0.0.1:5000/newsfor/hannah">http://127.0.0.1:5000/newsfor/hannah</a> one would see something like the following web page (although you can make it prettier, if you’d like, using CSS [see this week’s lecture slides for details of how]):










<strong><em>Print user’s name [4 points]</em></strong>

<ul>

 <li>Using Flask and a template, write a function bound to the /newsfor/&lt;name&gt; route that displays the “Hello, &lt;name&gt;!” at the top of the page for any name that follows /newsfor/ in the URL.</li>

 <li>Make sure the name is capitalized when it’s displayed on the page, even if the user types the URL in the browser in all lowercase. So, if I were to go to localhost:5000/newsfor/pedja it should still say “Hello, Pedja!” at the top of the page.</li>

 <li>To make this work, you will need to write an appropriate template file.</li>

</ul>




<strong><em>Query newsapi.org API for top 5 technology headlines [10 points]</em></strong>




In your top_headlines.py file, write code to retrieve the top 5 current technology headlines from the newsapi.org and display them for the user:

<ul>

 <li>To do this, you will need to access the newsapi.org API like we did in class earlier this term.</li>

 <li>In a file called secret.py, put your API key and name it like this:

  <ul>

   <li>API_KEY = “&lt;your api key&gt;”</li>

  </ul></li>

 <li>Format the top 5 articles with the corresponding titles linked to their URLs as an unordered (number) list.</li>

</ul>







———————————————————————————————————————




<strong>Extra Credit 1 – Make your Flask Application Interactive [2 points]</strong>

Update your top_headlines.py file to create another route /news/&lt;topic&gt; that will display top five current headlines for a topic of the user’s choice (e.g., science, sports, etc.). So, the user could go to <a href="http://localhost:5000/news/impeachment">http://localhost:5000/news/impeachment</a> and the system would give back a page with the title “Top news about impeachment” and then list top five headlines about impeachment. Note that you should be able to use the exact same template file for this part as you did for part 2 of the homework.




<strong>What to turn in:</strong>

<ol>

 <li>Upload your top_headlines.py file to Canvas</li>

 <li>Upload the screenshot of your working directory (for part 1)</li>

 <li>You <u>do not</u> need to upload your secret.py file. As long as you named your api key API_KEY, we should be able to run your code.</li>

</ol>