![](graphics/microsoftlogo.png)

# Lab: Python Basics for Data Professionals

#### <i>A Microsoft Course from the SQL Server team</i>

<p style="border-bottom: 1px solid lightgrey;"></p>

<dl style="text-align: left;">

  <dt><a href="#about">About this lab</a></dt>
  <dt><a href="#businessapplications">Business Applications of this lab</a></dt>
  <dt><a href="#technologies">Technologies used in this lab</a></dt>
  <dt><a href="#prereqs">Before Taking this lab</a></dt>
  <dt><a href="#details">lab Details</a></dt>
  <dt><a href="#related">Related labs</a></dt>
  <dt><a href="#modules">Lab Modules</a></dt>
  <dt><a href="#nextsteps">Next Steps</a></dt>

</dl>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/textbubble.png"> <h2><a name="about">About this lab</a></h2>

> NOTE: This course is in active re-development. [The course files are complete, and located here](https://github.com/microsoft/sqlworkshops-pythonfordatapros/tree/master/PythonForDataProfessionals), but this page is currently being worked on. 

Welcome to this Microsoft solutions lab on the architecture on *Python Basics for the Data Professional*. In this lab, you'll learn basic Python structures, programming and data flow. You'll get resources to go much further in your learning journey, but this short lab will get you up and running quickly. 

The focus of this lab is to familiarize the database professional in the basics of Python, while implementing it in SQL Server Stored Procedures using SQL Server's Machine Learning Services. After this basic introduction, the professional can move on to more in-depth training in Python if desired. 

You'll start by setting up your system to work with Python, then move to understanding the course itself. From there, you will move though programming basics, working with data, and then on to understanding the concepts of Python environments and how to deploy Python code.

This [github README.MD file](https://lab.github.com/githubtraining/introduction-to-github) explains how the workshop is laid out, what you will learn, and the technologies you will use in this solution. To download this Lab to your local computer, click the **Clone or Download** button you see at the top right side of this page. [More about that process is here](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository). 

You can view all of the [courses and other labs our team has created at this link - open in a new tab to find out more.](https://microsoft.github.io/sqllabs/)

<p style="border-bottom: 1px solid lightgrey;"></p>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/checkmark.png"> <h3>Learning Objectives</h3>

In this lab you'll learn:
- How to set up a Python environment for SQL Server using Machine Learning Services
- The Basics of programming in Python including code syntax, getting help, variables, operators, and functions 
- Working with data structures, and understanding popular data libraries
- Data Ingestion and access
- Machine Learning in Python
- Environments and code deployment

<br>

The goal of this lab is to familiarize the data professional with Python environments and programming. 

The concepts and skills taught in this lab form the starting points for:

  - Data professionals that wish to include Python code in their data access and programming
  - Security professionals who wish to understand how to securely implement secure Python coding practices
  - Anyone interested in learning more about programming with Python and databases

<p style="border-bottom: 1px solid lightgrey;"></p>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/building1.png"> <h2><a name="businessapplications">Business Applications of this lab</a></h2>

Businesses require the ability to securely access their data for many workloads, including various programming languages. Python (along with the R language) has merged as a powerful tool for data ingestion, processing and analysis. Previously, Python programmers accessed various databases and retrieved data over a network connection like any application, but this often means pulling large amounts of data over a potentially insecure network to bring multiple copies to each developer to work with locally. The SQL Server Machine Learning Services feature allows Python code to run inside a Stored Procedure in SQL Server, which then accesses data directly. This also allows the Python developer to create code locally, and then send that code on to the Database Administrator for installation on the server - the developer never has to touch the production server or data. 

This couse explains how to work with Python, and then how to operationalize the code on a SQL Server. 


<p style="border-bottom: 1px solid lightgrey;"></p>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/listcheck.png"> <h2><a name="technologies">Technologies used in this lab</a></h2>

The solution includes the following technologies - although you are not limited to these, they form the basis of the lab. At the end of the lab you will learn how to extrapolate these components into other solutions. You will cover these at an overview level, with references to much deeper training provided.

 <table style="tr:nth-child(even) {background-color: #f2f2f2;}; text-align: left; display: table; border-collapse: collapse; border-spacing: 2px; border-color: gray;">
  <tr><th style="background-color: #1b20a1; color: white;">Technology</th> <th style="background-color: #1b20a1; color: white;">Description</th></tr>
  <tr><td><i>Python</i></td><td>*An Open-Source, multiple paradigm coding language with extensible packages</td></tr>
  <tr><td><i>Microsoft SQL Server</i></td><td>*A complete data platform, including a Relational Database Management System (RDBMS), Data Pipeline, Business Intelligence, Graph Database Processing, and other constructs to work securely with multiple forms of data, including structured, semi-structured and unstructured.</td></tr>
 </table>

<p style="background:#ccc; color:#000;padding: 25px 25px 25px 25px;">

<p style="border-bottom: 1px solid lightgrey;"></p>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/owl.png"> <h2><a name="prereqs">Before Taking this lab</a></h2>

You'll need a local system that you are able to install software on. The lab demonstrations use Microsoft Windows as an operating system and all examples use Windows for the lab. Optionally, you can use a Microsoft Azure Virtual Machine (VM) to install the software on and work with the solution.

This lab expects that you understand data structures and working with SQL Server and computer networks. This lab does not expect you to have any prior data science knowledge, but a basic knowledge of programming and statistics is helpful.

If you are new to these, here are a few references you can complete prior to class:

-  [Microsoft SQL Server](https://docs.microsoft.com/en-us/sql/relational-databases/database-engine-tutorials?view=sql-server-ver15)
-  [Microsoft Azure](https://docs.microsoft.com/en-us/learn/paths/azure-fundamentals/)
-  [Basic Programming](https://www.khanacademy.org/computing/computer-programming/programming/intro-to-programming/v/programming-intro)

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/bulletlist.png"> <h3>Setup</h3>

<a href="SQL2019BDC/00%20-%20Prerequisites.md" target="_blank">A full prerequisites document is located here</a>. These instructions should be completed before the lab starts, since you will not have time to cover these in class. <i>Remember to turn off any Virtual Machines from the Azure Portal when not taking the class so that you do incur charges (shutting down the machine in the VM itself is not sufficient)</i>.

<p style="border-bottom: 1px solid lightgrey;"></p>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/education1.png"> <h2><a name="details">lab Details</a></h2>

This lab uses the Microsoft Windows operating system, although Linux is also supported once you have completed the exercises.

<table style="tr:nth-child(even) {background-color: #f2f2f2;}; text-align: left; display: table; border-collapse: collapse; border-spacing: 5px; border-color: gray;">

  <tr><td style="background-color: Cornsilk; color: black; padding: 5px 5px;">Primary Audience:</td><td style="background-color: Cornsilk; color: black; padding: 5px 5px;">Data Professionals tasked with implementing Big Data, Machine Learning and AI solutions</td></tr>
  <tr><td>Secondary Audience:</td><td> Security Architects and Developers</td></tr>
  <tr><td style="background-color: Cornsilk; color: black; padding: 5px 5px;">Level: </td><td style="background-color: Cornsilk; color: black; padding: 5px 5px0;"> 300</td></tr>
  <tr><td>Type:</td><td>In-Person</td></tr>
  <tr><td style="background-color: Cornsilk; color: black; padding: 5px 5px;">Length: </td><td style="background-color: Cornsilk; color: black; padding: 5px 5px;">8-9 hours</td></tr>

</table>

<p style="border-bottom: 1px solid lightgrey;"></p>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/pinmap.png"> <h2><a name="related">Related labs</a></h2>

 - This course is also availalbe in a zero-install, online Jupyter Notebook format. [You can find that here](https://notebooks.azure.com/BuckWoodyNoteBooks/projects/PythonDataProfessional).

<p style="border-bottom: 1px solid lightgrey;"></p>

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/bookpencil.png"> <h2><a name="modules">lab Modules </a></h2>

This is a modular lab, and in each section, you'll learn concepts, technologies and processes to help you complete the solution.

<table style="tr:nth-child(even) {background-color: #f2f2f2;}; text-align: left; display: table; border-collapse: collapse; border-spacing: 5px; border-color: gray;">

  <tr><td style="background-color: AliceBlue; color: black;"><b>Module</b></td><td style="background-color: AliceBlue; color: black;"><b>Topics</b></td></tr>

  <tr><td><a href="https://github.com/microsoft/sqlworkshops-pythonfordatapros/blob/master/PythonForDataProfessionals/01%20Overview%20and%20Course%20Setup.md" target="_blank">01 - Overview and Course Setup </a></td><td> In this Module you will cover and overview of the Python language and set up your system for the course.</td></tr>
  <tr><td style="background-color: AliceBlue; color: black;"><a href="https://github.com/microsoft/sqlworkshops-pythonfordatapros/blob/master/PythonForDataProfessionals/02%20Programming%20Basics.md" target="_blank">02 - Programming Basics</a> </td><td td style="background-color: AliceBlue; color: black;"> This Module covers the commands and procedures for getting help in Python, code syntax and structure, variables, and operators and functions.</td></tr>
  <tr><td><a href="https://github.com/microsoft/sqlworkshops-pythonfordatapros/blob/master/PythonForDataProfessionals/03%20Working%20with%20Data.md" target="_blank">03 - Working with Data </a></td><td> In this Module you will learn more about data types, ingestion, inpsection, and graphing, with a brief introduction to Data Science with Python.</td></tr>
  <tr><td style="background-color: AliceBlue; color: black;"><a href="https://github.com/microsoft/sqlworkshops-pythonfordatapros/blob/master/PythonForDataProfessionals/04%20Environments%20and%20Deployment.md" target="_blank">04 - Environments and Deployment</a> </td><td td style="background-color: AliceBlue; color: black;"> In this Module you will learn more about Python environments such as Conda, and how to deploy your code using the "pickle" library.</td></tr>
 
 </table>

<p style="border-bottom: 1px solid lightgrey;"></p>

<p><img style="float: left; margin: 0px 15px 15px 0px;" src="https://raw.githubusercontent.com/microsoft/sqlworkshops/master/graphics/geopin.png"><b><a name="nextsteps">Next Steps</a></b></p>

Next, Continue to <a href="https://github.com/microsoft/sqlworkshops-pythonfordatapros/blob/master/PythonForDataProfessionals/00%20Pre-Requisites.md" target="_blank"><i> 00 - Prerequisites</i></a>


# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

# Legal Notices

### License
Microsoft and any contributors grant you a license to the Microsoft documentation and other content in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode), see [the LICENSE file](https://github.com/MicrosoftDocs/mslearn-tailspin-spacegame-web/blob/master/LICENSE), and grant you a license to any code in the repository under [the MIT License](https://opensource.org/licenses/MIT), see the [LICENSE-CODE file](https://github.com/MicrosoftDocs/mslearn-tailspin-spacegame-web/blob/master/LICENSE-CODE).

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation
may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries.
The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks.
Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all other rights, whether under their respective copyrights, patents,
or trademarks, whether by implication, estoppel or otherwise.

