<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Installing / Enabling IIS
- Installing PHP Manager, Rewrite Module, and Creating a new directory 
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<p>
<img width="770" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/847d09d4-db4d-4a6e-86c0-fe052b068f61">

</p>
<p>
First, we are going to install and enable IIS (Internet Information Services) which allows our computer to serve up websites such as osTicket. By getting to our IIS we need to type control panel on the bottom left of our Windows search bar. From there click on programs then click on turn Windows features on or off. You should have something similar to the screenshot I provided above. Make sure to check off Internet Information Services, expand IIS, and make sure everything in common HTTP features are checked off so we have no errors, now go to applications development features and check off CGI which is a protocol for web servers to execute programs. Finally, click on the ok button to install everything, and to test it go to a web browser and type in 127.0.0.1 if you see a page about IIS, you are ready for the next steps.
</p>
<br />

<p>
<img width="386" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/3377f81c-2ac0-4d51-b4f1-b1791e8250f9">
<img width="385" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/eaf5620c-b87e-4627-a05c-8802a208cfaf">
<img width="839" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/087db7b5-e7f0-4005-8f5b-a5948e4596e1">



</p>
<p>
Next, we are going to install PHP Manager for IIS which is a free tool that helps you install, configure, and troubleshoot PHP on IIS. After you get done installing PHP Manager you now have to install Rewrite Module. Rewrite Module is a web server module that allows us to create rules to manipulate URLs so we can make friendly URLs for our users to remember and use. Now create the directory C:\PHP which you can go to your c drive in your file explorer and create a new folder and name it PHP.
</p>
<br />

<p>
<img width="440" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/e951be3e-1dd1-43f2-b7b6-af4da1104367">
<img width="359" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/e7b2e31d-e318-4d89-93f9-290546dcffba">


</p>
<p>
  <img width="371" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/17737856-e41e-4939-8736-6dd1441ad43a">
  <img width="372" alt="image" src="https://github.com/LeoHolguin/osticket-prereqs/assets/138087728/78f8db0b-d958-4ce3-9d40-84beae278e8e">

</p>

<p>
Then, we are going to download PHP 7.3.8 to our computer. Once it finishes downloading we need to extract all to inside our new PHP folder. Now download C++ redistributable which is a package that installs runtime libraries for C++ applications built with Microsoft tools. But for us, PHP requires it in order to run smoothly. Next, Install MySQL, make sure you click on typical setup and finish the installation. After that, you should get a configuration window to pop up, click on standard configuration and click next until you reach where you can put in a password. This is only lab so I'm going to put Password1 but of course, if this was in a real environment you should always have a complex password for security reasons. Finally, You should find a button to click execute and after that, you are done with MySQL. Basically, we downloaded a database where all the applications are going to be stored at.
</p>
<br /> 
