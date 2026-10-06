<img width="1700" height="1000" alt="55534921-0139-48d7-816b-0f3a75aa0d09" src="https://github.com/user-attachments/assets/d3b922f4-58fe-492f-9f2f-8a15a20136d3" />



# HelpDesk-Lab-osTicket-VM
This is a project where I built and installed a virtual IT helpdesk environment by using a virtual machine that I also created and configured and an osTicket system.
## 🛠️ Technologies & Tools

 Technology / Tool  Purpose 

☁️ Microsoft Azure
 
💿Operating System
 
 🎫osTicket
 
 🌐Web Server
 
📁File Services 


---

# 🖥️ 1. Virtual Machine Setup/Configuration


<details> 
 <summary>🏗️Building Virtual Machine</summary>
<img width="2556" height="1228" alt="Creating the VM" src="https://github.com/user-attachments/assets/a6255e81-4a9c-4627-aa98-403bcafae796" />
This is where I start the initial process of creating a virtual machine. I need to create a VM in order to install and osTicket system, Windows, IIS, and PHP without messing anything up on my actual computer or host computer. Here is also where we will set the username and password for the Admin Account.

---
  
<img width="948" height="1184" alt="Setting up VM" src="https://github.com/user-attachments/assets/dec529eb-06fc-4b20-b029-aa2110e50850" />
Here in this image I am setting up the hardware and configuration for the VM. I  do this because I need to make sure that the VM has enough memory, storage and processing power in order to be able to run the server software smoothly.

---

<img width="1024" height="1094" alt="VM network settings" src="https://github.com/user-attachments/assets/e4aec9ee-dabd-480f-ad04-c48c2d6e603f" />
Here is the VM's network configuration and I didn't actually have change anything on the step of building and configuring the VM, it was already setup how it needed to be. Now the VM is ready top be created.

---

<img width="2293" height="658" alt="VM being created" src="https://github.com/user-attachments/assets/80d95b7b-b5fc-4373-9aae-baa7cbe997e0" />
In this image we just see all of the deployments of the things I just configured in order to create the actual VM.

---

<img width="1759" height="702" alt="VM succesfully created" src="https://github.com/user-attachments/assets/1b716016-e36b-47ea-af24-d68ba32d2edf" />
This is after all the deployments have completed meaning that the VM has been successfully created.

---

<img width="2143" height="1228" alt="VM overview" src="https://github.com/user-attachments/assets/9d3d3950-52e2-47e4-b9a8-c811fca3b49c" />
This is a screenshot of the VMs overview showing a bunch of information about the VM and its properties, such as the IP Address which I will actually be needing.

---

<img width="1999" height="675" alt="using RD to log into the vm" src="https://github.com/user-attachments/assets/c7565279-b31b-4379-8f63-03433018927f" />
Here is where we use Remote Desktop to log into the VM buy getting its IP Address and connecting Remote Desktop to that VM specifically. This is where we need those Admin Account credentials we created and so we put that information in here.

<img width="2035" height="681" alt="Logging into VM" src="https://github.com/user-attachments/assets/08c53826-56f3-4163-83c2-5ac2422ea2ff" />
This is the very next page that we get if we put in the correct information to log into the VM Admin Account. Its just telling us the identity of the VM can't be determined which is fine because I created it. This is the last step in the setup, configuration, and creation  of a VM for the use of creating a osTicket system. The next step will take me into the VM where I will begin the process of configuring and creating the osTicket system.

</details>

# 🎫 2. osTicket Installation and Setup


<details>
 <summary>🏛️ Building & Configuring osTicket System</summary>
<img width="2523" height="338" alt="Downloading OsTicket Files on VM" src="https://github.com/user-attachments/assets/463f5e5e-d62c-4904-87a0-d1ebe57e1f9c" />
 This is the first step in setting up the osTicket system. I had to go download all the files I will need in order to allow and make sure the ticketing system actually works, without these application files the osTicket system wouldn't be able to work.
 
 - - - 
 
<img width="1775" height="1000" alt="Extracting the OsTicket files" src="https://github.com/user-attachments/assets/349113c0-81d1-4ed7-8b00-9f5280f31b85" />
After downloading all of the application files I needed I now needed to extract all the files out of the zipped folder so here is me doing that by right clicking on the file and then selecting extract all. This essentially just creates a new folder that ahs all the files that were in the zipped folder but now you can open it and access those files.

---
<h2> 🌐IIS</h2>
<br>
<br>
<br>

<img width="1124" height="636" alt="Going into Control   Panel to enable IIS" src="https://github.com/user-attachments/assets/c16a178b-dcea-46bc-a19d-3811cf61db92" />
The next thing I did after extracting the files was I went into the control panel in order to enable Internet Information Services or IIS.

<img width="1121" height="628" alt="Going into programs on CP" src="https://github.com/user-attachments/assets/b2b68905-578e-4d49-bda0-baa92dab9c91" />
Once we get into the Control Panel we have to navigate to the programs so we click on programs and then we get taken to the screen you see here now on this screen we need to slick onto turn windows optins on or off this is so we can enable IIS.

<img width="1126" height="628" alt="Turning on Windows features" src="https://github.com/user-attachments/assets/299dc1b4-24cb-4a63-b5f9-69182a163b2b" />
In this screenshot this is what I see when I first opened up windows features.

<img width="1124" height="634" alt="Turning on IIS and CGI in CP" src="https://github.com/user-attachments/assets/e8ae9aaf-989a-4f53-93e1-ea76c8dd6e2f" />
This is where after getting into this windows features page I navigated to IIS and checked its box I then expanded its folder to then expand the world wide web services folder and finally expanding the application development features folder to find CGI and to make sure it is checked. CGI basically allows the IIS to communicate with the PHP.

---
<h2>🅿️ PHP Setup </h2>
<br>
<br>
<br>
<img width="1117" height="623" alt="Installing PHP manager on VM" src="https://github.com/user-attachments/assets/f42054f7-0c7d-420b-bcad-e9b8122908fe" />
The next step I need to take to create this osTicket system is to install the PHP manager. This is showing where in the folder that we unzipped earlier all the application files we are going to need are, so I click on the PHP manager to install it.
<img width="499" height="411" alt="PHP Menu 1" src="https://github.com/user-attachments/assets/716aca16-9656-4f28-8c9d-f33fc33203a9" />
<img width="504" height="404" alt="PHP License Agreement" src="https://github.com/user-attachments/assets/d1403b51-7e17-4b03-a1c1-0cc156c81bc8" />
<img width="500" height="414" alt="PHP Manager Successfully installed" src="https://github.com/user-attachments/assets/8696342d-0958-471c-a411-48eddb41b850" />

These three pictures are all showing the navigation through the installing menus of the PHP manager. So when downloading this, I just hit next and then accepted the terms and hit next and now it s installed.

---
<h2>🔄️ ISS Rewrite Install</h2>
<br>
<br>
<br>
<img width="1125" height="630" alt="Installing Rewrite File on VM" src="https://github.com/user-attachments/assets/a456893d-2456-49fd-baa0-d4284428d498" />
Here is me doing essentially the same thing as the PHP manager but for the rewrite file this time so I am goin into the application files and installing the rewrite file.
<br>

<img width="489" height="390" alt="Accepting Rewrite Terms and Installing" src="https://github.com/user-attachments/assets/384de029-cf34-4cec-8608-e680dbebb461" />

<img width="495" height="382" alt="Rewrite Successfully Installed" src="https://github.com/user-attachments/assets/dd1d196f-cf22-447f-b547-1620c1e62b91" />

Here are the menus for when you go through installing the rewrite file. No configurations needed so I just had to accept terms and then click install then it was finished.

---
<h2>🏫 Testing and Installing PHP</h2>
<br>
<br>
<br>
<img width="1125" height="629" alt="Going to C drive to Create PHP file" src="https://github.com/user-attachments/assets/ee6ecadb-fc9e-4e6e-baee-d9e258e301ad" />
This is the beginning of the next step which is creating a PHP file on the VMs C drive. This is me going to file explorer to navigate to the C Drive.

<img width="1124" height="632" alt="Going to VMs C drive To Create PHP file" src="https://github.com/user-attachments/assets/34a73199-16ac-49d8-9f63-819a4d49026c" />
Here I am going to This PC in order to find the C Drive.

<img width="1120" height="633" alt="Created PHP File" src="https://github.com/user-attachments/assets/99c3e5ea-1013-4bda-8d6b-f2d703ceacf0" />
So here is when I get to the C Drive and then create a new folder named PHP and we needed to do this so we have a place to put all the PHP files in our application files we downloaded into this file.

<img width="1129" height="758" alt="Extracting PHP files from osticket File into C Drive PHP Folder" src="https://github.com/user-attachments/assets/69167e14-d803-4819-b17f-775f2faa6067" />

Next we need to extract the files from this folder but this time we need to make sure they go into a specific folder.

<img width="612" height="451" alt="Browsing to C Drive PHP Folder" src="https://github.com/user-attachments/assets/8d28c5c2-8bf9-44e4-bd32-e0fe2689f112" />

Now this is where I can select where these files are going to go once they are extracted. So I hit browse on this screen to go and find the PHP file I just created.

<img width="610" height="458" alt="Selected PHP Folder For PHP File Extraction" src="https://github.com/user-attachments/assets/7cb8fc8a-48b2-4b53-b155-540d449bd1e8" />

Here is when I select the PHP folder on the VMs C Drive and that means that all the files we're extracting will now be in that folder.

<img width="1121" height="636" alt="Files Successfully extracted into PHP folder" src="https://github.com/user-attachments/assets/5f4b2186-6743-4c18-815b-ae148c60a80f" />
To make sure the files went to the correct place and nothing got messed up I went back into file explorer and went to the PHP files and this image show they were extracted successfully.

---
<h2>📼 VC Installation</h2>
<br>
<br>
<br>
<img width="1123" height="630" alt="Installing VC for VM" src="https://github.com/user-attachments/assets/dc45292e-6e8e-4a28-abe5-4cf2dabcfbbf" />
This is the next installation I have to make and that is the VC application. Here is me clicking on it in order to start the installation process.
<br>
<img width="475" height="300" alt="Agreeing to VC terms and Installing" src="https://github.com/user-attachments/assets/00a3a79e-3569-400a-951c-3e1973de763b" />
<img width="477" height="298" alt="VC successfully Installed" src="https://github.com/user-attachments/assets/71cba6c5-7225-4c17-8c32-ec299453d715" />

These two images are the menus you see when installing the VC, its just accepting terms and then selecting install and then showing install is complete.

---
<h2>🐬 MySQL Database</h2>
<br>
<br>
<br>
<img width="1132" height="641" alt="Installing mysql on VM" src="https://github.com/user-attachments/assets/2224c6d6-8cd5-43dc-952e-24d6ab10b40b" />
Now in this screenshot I am installing mysql. This is me clicking on it to start the installation process.
<br> 
<br>
<br>
<img width="496" height="390" alt="mysql setup 1" src="https://github.com/user-attachments/assets/d93d9658-5aee-4eda-bf45-64dd736bebe3" />
<img width="492" height="387" alt="Agreeing to mysql Temrs and Continuing" src="https://github.com/user-attachments/assets/0201917e-35fe-483a-a609-ff6e04c2808b" />
<img width="496" height="386" alt="Selecting Typical for mysql" src="https://github.com/user-attachments/assets/01598fb5-48e0-4000-8389-0e39a1a5230a" />
<img width="499" height="391" alt="Installing mysql final step" src="https://github.com/user-attachments/assets/90a71f2c-3a23-4b88-86a8-39731c331eb2" />
<img width="494" height="388" alt="mysql install completed" src="https://github.com/user-attachments/assets/8543d162-1d87-47a9-8ab9-3b24d02d900a" />
<img width="498" height="381" alt="mysql wixard setup after install" src="https://github.com/user-attachments/assets/795c34df-2b64-4ee6-9485-ed86543e17d4" />
<img width="496" height="379" alt="mysql standard configuration setup after install" src="https://github.com/user-attachments/assets/c9f1041a-8b0c-4196-974b-bc16eed97679" />
<img width="500" height="379" alt="mysql setting up root password" src="https://github.com/user-attachments/assets/5a83937a-06d0-4bbb-8e4c-8a533bc23de1" />
<img width="494" height="383" alt="mysql executing configuration" src="https://github.com/user-attachments/assets/adbe11ac-7cc9-4b60-92dc-df362b0e695c" />
<img width="500" height="377" alt="mysql configuration execution completed" src="https://github.com/user-attachments/assets/226cdd71-97f6-4340-9a1d-8cba05786ae6" />
All these photos are doing the installation and configuration process of mysql. The important things while installing this were making sure I picked typical for the setup type making sure during the configuration I chose standard and then finally the most important thing not forgetting the root password as we will need it later and if we dont have it it will break the whole osTicket system.

---
<h2>🪢 Connecting PHP to IIS</h2>
<br>
<br>
<br>
<img width="836" height="453" alt="Running IIS as admin on VM" src="https://github.com/user-attachments/assets/ae469bf4-6485-429d-9a39-e6bd9eb1b4b4" />
The next thing I had to do is running IIS but making sure that I am running it as an administrator. This image shows me running IIS as an Admin.

<img width="1902" height="1012" alt="Going into PHP manager in IIS" src="https://github.com/user-attachments/assets/b062bb36-f8a7-4e27-b643-af90c487b4d9" />
This next image shows me navigating to the PHP manager in IIS.

<img width="1697" height="662" alt="Registering a new PHP version" src="https://github.com/user-attachments/assets/b79d5c2e-3b05-4707-a467-92988eacae23" />
Now that I am in the PHP manager I am now going to register a new PHP version. This is showing that I now have to go and provide a path for the PHP-CGI.

<img width="1182" height="708" alt="Browsing to PHP Folder On C Drive in IIS" src="https://github.com/user-attachments/assets/685bac7f-d72e-4699-872f-d19541319751" />
Here is me going into the C Drive in order to find that PHP file I created earlier and extracted all those files into. 

<img width="1185" height="708" alt="Selecting PHP cgi to  register new PHP in IIS" src="https://github.com/user-attachments/assets/7f889c49-0a4f-4d5a-b646-2c190612b521" />
Next after navigating to the PHP folder I then select the php-cgi file to create that pathway for the IIS. 

<img width="1699" height="282" alt="Reloading IIS server By stopping it " src="https://github.com/user-attachments/assets/40930bed-db8f-426d-848b-85e1b162d765" />
<img width="1691" height="290" alt="Reloading IIS server by Starting it" src="https://github.com/user-attachments/assets/27e0e0b3-fa48-4cc9-a380-a6c3ca7d44ec" />
These two screenshots show me stoping and then starfting the IIS server in order to reload it so it uses that new PHP I just registered.

---
<h2>🧪 Placing and testing osTicket in IIS</h2>
<br>
<br>
<br>
<img width="1134" height="578" alt="Extracting OsTicket Folder for Install" src="https://github.com/user-attachments/assets/ff848b6a-d587-4629-834f-4c1359f148f9" />
In this image it shows me clicking on the osTicket folder in order to extract the files in the zipped folder.

<img width="1122" height="635" alt="Going to VMs C Drive to navigate to the inetpub folder" src="https://github.com/user-attachments/assets/eea8680e-286b-4aa1-89f0-f835a4eb71ed" />
This image shows me navigating to the inetpub folder in the C Drive because I need to find the wwwroot folder and it is in this folder.

<img width="1123" height="634" alt="Going into inetpub folder  to get into the wwwroot folder" src="https://github.com/user-attachments/assets/8bfe8231-26a9-45b0-b969-9c517ce54e48" />
Now that I am in the inetpub folder I see the wwwroot folder which is the folder I need in order to put the upload folder from the osTicket folder into it.

<img width="2259" height="722" alt="copying upload folder into the wwwroot folder" src="https://github.com/user-attachments/assets/b29bfc6d-4950-419f-b569-2e65ee0ed0b2" />
Here is the image showing both of the folders after I found the wwwroot folder and before I take the upload folder out of the the osTicket folder and putting it into the wwwroot folder.

<img width="2251" height="704" alt="upload folder copied into wwwroot folder" src="https://github.com/user-attachments/assets/d3a88296-d165-47d1-b0de-07141a1e1fa4" />
This image is showing after I moved the upload folder from the osTicket folder into the wwwroot folder.

<img width="1125" height="637" alt="renaming upload folder to osTicket " src="https://github.com/user-attachments/assets/95dc7bed-6ad9-40ab-b73c-2ea10885abdf" />
Now the next thing I do with the folder after moving it is renaming it to "osTicket" which is what I am doing in this image.

<img width="1902" height="493" alt="Going in IIS to attempt to browse to osTicket" src="https://github.com/user-attachments/assets/459bcfc7-3fc6-423a-a335-583bf4c9854f" />
This screenshot shows me going back into the IIS manager to se if I can now browse to the osTicket

<img width="1911" height="512" alt="Browsing to osTicket in IIS to open it" src="https://github.com/user-attachments/assets/18c26834-8389-41f7-be89-f6ca0c5636d6" />
Now that I am in IIS manager this is the next step in order try and find the osTicket and browse to it. I had to navigate through the Sites drop window and then default web site drop window and there is our osTicket folder. I then clcik on the folder and then on the right it says browse *:80(http) so I then click on it to see I can browse to the osTicket system.

<img width="2466" height="946" alt="osTicket sauccessfully browsed to" src="https://github.com/user-attachments/assets/ab390c17-f21f-42bc-bd18-cdeece682a6e" />
This is the webpage I went to after browsing to the osTicket system meaning it was successful and the webpage is browseable. As the photo shows though there are some extensions missing that will allow me to use all the features of the osTicket system.

---
<h2>🧩 Enabling PHP Extensions</h2>
<br>
<br>
<br>
<img width="1903" height="1013" alt="Going to PHP manager through the osTicket default website in IIS" src="https://github.com/user-attachments/assets/d8a2ce4d-ccde-4488-9641-64bc68db6e1e" />
Going back to the IIS where we are on the osTicket folder this is showing me go into the PHP for the osTicket system directly.

<img width="639" height="586" alt="Going into  PHP extensions to enable extensions for osTicket" src="https://github.com/user-attachments/assets/d5488eab-c3ba-44d8-b4bf-f3f7a77c5540" />
 This is the page that I am brought to after going into the osTicket PHP manager. This also shows the PHP extensions which is where I am navigating to.
 
<img width="1506" height="919" alt="Navigating into the PHP extensions" src="https://github.com/user-attachments/assets/7e9f63bf-e992-40b0-95bb-278465a36494" />
This photo is showing the page with all the extensions for the osTicket and I am looking for three specific ones which are imap.png, intl.dll.png, and opcache.dll.png
<br>
<br>
<br>
<img width="769" height="1005" alt="Enabling PHP imap" src="https://github.com/user-attachments/assets/baf3a206-6b37-4c0d-8951-b8d2e2cddc38" />
<img width="792" height="1018" alt="Enabling PHP intl dll" src="https://github.com/user-attachments/assets/091e0839-e010-42d5-90cc-2ac06f6126c5" />
<img width="774" height="1012" alt="Enabling PHP opcache dll" src="https://github.com/user-attachments/assets/9fa029f4-8b36-4401-beb8-2b3a7403b155" />
These last three screenshots are me showing how I enabled all three of those extensions I was looking for. 

<img width="2518" height="850" alt="Cinfirming extensions have been enabled on osTicket" src="https://github.com/user-attachments/assets/9c050154-8dcb-4d19-8f54-3aa6f36583e0" />
I finally went back into the web browser back to the osTicket system to make sure the extensions were enabled and as seen in this image they are now enabled successfully.

---
<h2>🔐 osTicket Configuration File/Permissions</h2>
<br>
<br>
<br>
<img width="1123" height="631" alt="going into osTicket folder in wwwroot folder to change name of file" src="https://github.com/user-attachments/assets/581a906f-b527-4c88-a8b7-1149f2fffd71" />
This next image is showing me beginning the next step of setting up the osTicket system which is going into the wwwroot folder and looking for a specific file in order to change its name.

<img width="1126" height="637" alt="Going into include folder in osTicket Folder" src="https://github.com/user-attachments/assets/8c80366c-8c20-4d85-8e24-c7857d3a5e54" />
Now that I am in the osTicket folder and I need to go into the include folder to find the file I need to rename

<img width="1119" height="633" alt="Finding ostsampleconfig file inside of include folder to change name" src="https://github.com/user-attachments/assets/37771a6f-993b-4e0a-8e2b-cd3e0cfdf947" />
Finally I am in the folder where the file is located and so I found it and am showing what it was named before I changed it in this picture.

<img width="1124" height="630" alt="changing ostsmapleconfig to ostconfig" src="https://github.com/user-attachments/assets/34d52ef2-d9be-4b20-aadb-08c2b4f568f2" />
In this picture it shows what that I renamed ostsampleconfig to ostconfig.

<img width="808" height="880" alt="Going to ost config properties" src="https://github.com/user-attachments/assets/17f453d0-a4ef-4a08-85f5-e226d4d277ee" />
After I renamed the file I then right click on it and am navigating to its properties in this image/

<img width="404" height="510" alt="going into securityt properties for ostconfig" src="https://github.com/user-attachments/assets/2d57ec0d-799b-4d61-b7e2-f7ad26897de1" />
Now that I am in the properties of that file in this image I then go into the security tab of the properties because I am trying to ensure the web application can access the configuration file for this lab.

<img width="769" height="516" alt="ostconfig advanced securitry properties" src="https://github.com/user-attachments/assets/38381f2c-0f7c-4f4e-9781-3b76c82c0b7e" />
After navigating to the security properties I then selected the advanced security options and this is an image of the window that came up.

<img width="762" height="510" alt="Disabling ostconfig inheritance" src="https://github.com/user-attachments/assets/169825a6-4743-48f5-b5c8-db61c4b4c777" />
The first thing I do in the is image is disabling inheritance meaning that this will not have any permissions applied to it through any parent objects. So on this screen I selected remove all inherited permissions from this object.

<img width="765" height="523" alt="removed all ostconfig inheritance" src="https://github.com/user-attachments/assets/d4a3631c-683e-40ed-9217-fbb7921fefcc" />
This a screenshot of after I removed all inherited permissions and since there are none I am going to add a new one so I click the add button.

<img width="917" height="594" alt="Adding new permission for ostconfig" src="https://github.com/user-attachments/assets/a113f42f-e393-4b9e-bc1a-c9dbb5fb4cb1" />
Once navigated to the window in the screenshot I then go to select a principal which will take me to another window.

<img width="470" height="282" alt="giving everyone access or permission to ostconfig" src="https://github.com/user-attachments/assets/93f30689-f93c-428e-a971-e092a1208226" />
This is the window that I am taken to after selecting a principal and I then type everyone which gives everyone access to this file.

<img width="606" height="452" alt="Giving everyone full cotrol of ostconfig" src="https://github.com/user-attachments/assets/b63fb870-5965-4bf0-b688-08101d8b92e4" />
In this photo it shows me giving everyone not only access but full control for ost-config.php
<img width="767" height="522" alt="Everyone has control of ostconfig" src="https://github.com/user-attachments/assets/f4383cb0-5dcb-47a7-9f0b-48232827a4d3" />
This is just an image of me confirming that everyone has full control of ost-config.php before I apply the changes to the permissions.

---
<h2>🎟️ Completing osTicket</h2>
<br>
<br>
<br>
<img width="2478" height="968" alt="Continuing osTicket setup in browser" src="https://github.com/user-attachments/assets/9ed92e5c-b85c-4bc1-a86a-38baa39cda4c" />
This is showing mew going back to the browser of the osTicket system and then hitting continue at the bottom to configure the osTicket system further.

<img width="846" height="1190" alt="osTicket setup in Browser" src="https://github.com/user-attachments/assets/c59e7e2c-910b-48fa-a0d5-6fe2eb06648e" />
This is an image of the webpage after I hit continue from the picture. I went ahead and filled all opf this information out which isnt super important for the lab but this is where you setup the Admin user and also the helpdesks name and things like that.

---
<h2>🗄️ HeidiSQL Installation and DataBase</h2>
<br>
<br>
<br>
<img width="1117" height="633" alt="Installing heidisql" src="https://github.com/user-attachments/assets/2cd144f8-ecce-4cd5-8418-624e0dc02006" />
Before finishing that osTicket configuration page we have to install I final thing which is heidisql. This is showing me starting that process by clicking on it in the application installation files.

<img width="595" height="461" alt="accepting heidi terms and continuing" src="https://github.com/user-attachments/assets/9d85596c-e606-4e66-8f33-c948dc602c71" />
<img width="596" height="464" alt="heidi setup 1" src="https://github.com/user-attachments/assets/0773372d-80a2-49a5-8a50-67d0f240d403" />
<img width="592" height="468" alt="heidi setup 2" src="https://github.com/user-attachments/assets/f5a8dddf-f71b-4ed6-a407-3c2fe4e1c3f2" />
<img width="591" height="465" alt="heidi setup 3" src="https://github.com/user-attachments/assets/ae693cc3-7382-4f41-81c5-a9d76e10de9d" />
<img width="592" height="466" alt="heidi final step installing" src="https://github.com/user-attachments/assets/5401989b-92ca-480f-8049-3a5296a181a9" />
<img width="595" height="466" alt="heidi finished installing and launching" src="https://github.com/user-attachments/assets/7768fe6b-09cf-43fa-86ca-4926424e66ec" />
All of these photos are showing the steps and process of installing heidisql but all I did was hit next and leave all the configurations as they were, and then clicking finish at the end.

<img width="424" height="754" alt="Heidi creating a new root session" src="https://github.com/user-attachments/assets/6cd5c25f-57d0-4230-8e54-080340269df0" />
So after setting up and installing heidisql it automatically opens up into this window where I am clicking on new at the bottom to create a new root session.

<img width="1109" height="747" alt="Setting up new root session in heidi" src="https://github.com/user-attachments/assets/d4ff9cd3-2d54-4f6c-82ef-7793c7a7ff80" />
This image is showing my setting up and configuring the new root session and this is where the password and username I made come back into play so I put in the user and password and hit open.

<img width="935" height="596" alt="heidi session from new session" src="https://github.com/user-attachments/assets/f6eb39b3-f9e6-41c0-9ea6-3b0af119faaf" />
This is the new root session being opened which means that it is working.
<img width="487" height="592" alt="creating new database for osTicket in heidi" src="https://github.com/user-attachments/assets/72856aa5-bad2-45a6-8d60-a0b40f22a3c6" />
In this screenshot it shows me right clicking on the part of the menu that says unnamed in order to create a new data base and so I do that and click on create new.

<img width="939" height="593" alt="naming new database for osTicket in heidi" src="https://github.com/user-attachments/assets/f0cab195-5085-4ba0-8c4f-ce04016ba8c4" />
This is showing me name the new data base I am creating which is going to be osTicket and it has to be exactly that because that is what we named that file in the root folder, after renaming it I hit ok.

---
<h2>✅ Final installation and Verification</h2>
<br>
<br>
<br>
<img width="852" height="1184" alt="Finishing osTicket in browser and installing it" src="https://github.com/user-attachments/assets/6859e880-2d6e-4d80-ab53-37f9126cc803" />
Here is the image of me finishing the configursatin for the osTicket system and putting in all the new info we just created in the bottom section.

<img width="830" height="653" alt="osTicket Installed" src="https://github.com/user-attachments/assets/b3abc967-681c-4c66-97b4-24dee929c581" />
This is just the congratulations screen you get when you installed and configured the osTicket system.

<img width="986" height="1136" alt="Confirming osTicket works" src="https://github.com/user-attachments/assets/801118ab-e47e-4b6d-b4d2-9e63282abc53" />
This is the final step of the lab which is me going into and signing into the osTicket system to confirm that it is working and it indeed is as in the picture.

 
</details>
