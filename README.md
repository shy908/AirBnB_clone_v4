Resources
Read or watch:

Selector
Get and set content
Manipulate CSS classes
Manipulate DOM elements
Document ready
Introduction
GET & POST request
HTTP access control (CORS)
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

General
How cool it is to request your own API
How to modify an HTML element style
How to get and update an HTML element content
How to modify the DOM
How to make a GET request with JQuery Ajax
How to make a POST request with JQuery Ajax
How to listen/bind to DOM events
How to listen/bind to user events
Copyright - Plagiarism
You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work.
You are not allowed to publish any content of this project.
Any form of plagiarism is strictly forbidden and will result in removal from the program.
Requirements
General
Allowed editors: vi, vim, emacs
All your files will be interpreted on Chrome (version 57.0)
All your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
Your code should be semistandard compliant with the flag --global $: semistandard *.js --global $
All your JavaScript must be in the folder scripts
You must use JQuery version 3.x
You are not allowed to use var
HTML should not reload for each action: DOM manipulation, update values, fetch data…
GitHub
There should be one project repository per group. If you clone/fork/whatever a project repository with the same name before the second deadline, you risk a 0% score.

More Info
Import JQuery
<head>
    <script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
</head>
Before starting the project…
You will work on a codebase using Flasgger, you will need to install it locally first before starting the RestAPI:

$ sudo apt-get install -y python3-lxml
$ sudo pip3 install flask_cors # if it was not installed yet
$ sudo pip3 install flasgger
If the RestAPI is not starting, please read the error message. Based on the(ses) error message(s), you will have to troubleshoot potential dependencies issues.

Here some solutions:

jsonschema exception
$ sudo pip3 uninstall -y jsonschema 
$ sudo pip3 install jsonschema==3.0.1
No module named 'pathlib2'
$ sudo pip3 install pathlib2
Expose ports from your Vagrant
In your Vagrantfile, add this line for each port forwarded

# I expose the port 5001 of my vm to the port 5001 on my computer
config.vm.network :forwarded_port, guest: 5001, host: 5001 
if you need to expose other ports, same line but you will need to replace the “guest port” (inside your vagrant) and your “host port” (outside your vagrant, used from your browser for example)

It’s important in your project, to use the AirBnB API with the port 5001