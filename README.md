# windows-serv-prov
<h1>Provisioning Windows Server 2019</h1>

<h2>Description</h2>
This project contains the step by step process through which my Windows Server 2019 VM was provisioned in my VirtualBox Home Lab
<br />

<h2>Utilities Used</h2>

- <b>VirtualBox</b> 
- <b>Windows Server 2019 OSI Image</b>

<h2>Environments Used </h2>

- <b>Windows Server 2019</b>

<h2>Lab walk-through:</h2>

<p align="center">
Launch VirualBox > Click New > Name your Server > Include the ISO Image: <br/>
<img src="https://imgur.com/piMLu8h.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Set Memory and Processor Preferences: I used 2GB of RAM and selected 2 core processors for the purpose of efficiency <br/>
<img src="https://imgur.com/gwNxLWr.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Setting Virtual Hard Disk to the default size of 50 GB: <br/>
<img src="https://imgur.com/joyCSeY.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Confirm selection and click "Finish":  <br/>
<img src="https://imgur.com/1wVT1se.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Click "Start" (green arrow ->) at the top of the VM and start provisioning the VM:  <br/>
<img src="https://imgur.com/G6L9CVn.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
When you click "Next" in the step above, you can click "Install Now". Here, there are 4 options regarding the type of experience to use. I selected "Desktop Experience" so that I could have both the GUI (Graphical User Interface) and the Command Line Option<br/>
<img src="https://imgur.com/x223k1s.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Selected Custom Install on the next page so that the hard drive can be formatted and we can start from scratch. Can go with the other option if you're installing a second time and have the required files available <br/>
<img src="https://imgur.com/gl9lBfq.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Installing.. The server will restart quite a bit at this stage and you will see something like press any key to boot from CD. No action is required here <br/>
<img src="https://imgur.com/EMQM0Oh.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Click Restart now <br/>
<img src="https://imgur.com/iv4ZNOR.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Set Admin account password and click Finish: <br/>
<img src="https://imgur.com/8F1od1U.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
For this I just clicked Input > Keyboard > Insert Ctrl-Alt-Del and it unlocked. If you can click the combination on your keyboard, that'll be faster and easier <br/>
<img src="https://imgur.com/209XOAX.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Signed in with Password created above and I'm in :) Selected 'Yes' for the Network Setting<br/>
<img src="https://imgur.com/RbGBSDJ.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
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
