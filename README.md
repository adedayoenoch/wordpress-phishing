<h1>Wordpress Phishing Page</h1>


<h2>Description</h2>
In this project, I will be explaining the whole process on how I used Gophish framework to create a very convincing wordpress phishing email. The following steps I will be showing can be replicated and used on any other login pages of your choice. I wont be showing how I setup Gophish to save time and if you need help setting it up, there's a lot of resources on youtube and chatgpt which should guide you through the whole setup. So without further delay I'll begin the project.
<br />


<h2>Environments Used </h2>

- <b>Windows 10</b> 

<h2>Program walk-through:</h2>

<p align="center">
First of all you'll need to start Gophish through the exe file: <br/>
<img src="https://i.imgur.com/bhs1zYn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Open your local host with the default config address at http://127.0.0.1:3333. Note that 3333 is the default port you'll be using to access gophish and it can be changed to your prefered port:  <br/>
<img src="https://i.imgur.com/8Mk6WjQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the login page: <br/>
<img src="https://i.imgur.com/01pUptZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
At first when setting up, you'll be given a username and password which will display on your windows terminal but I've already reset mine :  <br/>
<img src="https://i.imgur.com/fDcKbtN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Here's my dashboard:  <br/>
<img src="https://i.imgur.com/CGhH32c.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Since we are creating a wordpress phishing email, lets create a new group called wordpress:  <br/>
<img src="https://i.imgur.com/QCeidaH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Now we'll need a template from wordpress so it seems authentic :  <br/>
<img src="https://i.imgur.com/iCrBdGR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Lets import this email I got from wordpress :  <br/>
<img src="https://i.imgur.com/w1XHHes.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Lets get the source code :  <br/>
<img src="https://i.imgur.com/IEN4MuB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
We'll copy the source code in other to import it as our email template :  <br/>
<img src="https://i.imgur.com/YHMWAme.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Import :  <br/>
<img src="https://i.imgur.com/Z5Q02KE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
It automatically updates the subject and displays a mini page of how the email looks:  <br/>
<img src="https://i.imgur.com/MUuKXh6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Let's save the template:  <br/>
<img src="https://i.imgur.com/zvV4NQI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Lets create the landing page, the landing page is the site where the person that clicks the link in the email would be directed to :  <br/>
<img src="https://i.imgur.com/AjjAALV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Paste a link to the login page you want to spoof. I'll paste in the URL for wordpress:  <br/>
<img src="https://i.imgur.com/vBYWZ0L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
   <br />
The wordpress landing page should be displayed on a mini screen just like the email template was displayed:  <br/>
<img src="https://i.imgur.com/wcjtP3M.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> <br />
In order to make the victim unaware that he's been phished, we'll have to redirect him to the real login page of wordpress:  <br/>
<img src="https://i.imgur.com/KkqNBfE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> <br />
Lets create our sending profile, you can copy and paste my input... If you need more knowledge on smtp you can check out various smtp hosts on their page:  <br/>
<img src="https://i.imgur.com/bfmCOAA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> <br />
You can send a test email to confirm that the configurations to the sending profile were set properly :  <br/>
<img src="https://i.imgur.com/0zPcVbJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> <br />
We're almost done, we'll just set up our phishing campaign, its basically combining all the information we provided previously. For the URL, we'll use our local host URL :  <br/>
<img src="https://i.imgur.com/i84XLGb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> <br />
 Theres the email... you can use a spoofed email though, i just decided to use mine:  <br/>
<img src="https://i.imgur.com/Lnsz5kD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> 
<br />
There's the page, we can host it using a vps or buy a domain name from name cheap, keep in mind that hosting a phishing page is illegal. We can also edit the URL with a URL shortener:  <br/>
<img src="https://i.imgur.com/aNygG6j.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br /> <br />
Open your dasboard to see phishing success:  <br/>
<img src="https://i.imgur.com/K8IuD7G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Here's the phishing information and highlighted is the wordpress username and password I input in the spoofed page:  <br/>
<img src="https://i.imgur.com/F0pEnrb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
