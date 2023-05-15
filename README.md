<h1>Provisioning Windows Server 2019</h1>

<h2>Description</h2>
This project contains the step by step process through which my Windows Server 2019 VM was provisioned in my VirtualBox Home Lab
<br />

<h2>Utilities Used</h2>

- <b>VirtualBox</b> 
- <b>VirtualBox Guest Additions</b> (can be downloaded on the VirtualBox website)
- <b>Windows Server 2019 ISO Image</b>

<h2>Environments Used </h2>

- <b>Windows Server 2019</b>

<h2>Acronyms Used (in order of appearance) </h2>

- <b>VM: Virtual Machine</b> 
- <b>GUI: Graphical User Interface</b>
- <b>CLI: Command Line Interface</b>
- <b>CD: Compact Disk</b>
- <b>DC: Domain COntroller</b>
- <b>NAT: Network Address Translation</b>
- <b>NIC: Network Interface Card</b>

<h2>Lab walk-through:</h2>

<p align="center">
Launch VirualBox > Click New > Name your Server > Include the ISO Image. This tells your box where to "pick" or "load" the server 2019 image from: <br/>
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
When you click "Next" in the step above, you can click "Install Now". Here, there are 4 options regarding the type of experience to use. I selected "Desktop Experience" so that I could have both the GUI and the CLI option<br/>
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

<h2>Some Housekeeping :) </h2>
This helps make the experience better on the box level and the VM level
<br />

<p align="center">
<b> From your Box (Ensure your VM is powered off for this):</b> Click Settings > General > Advanced > Select "Bi-directional" for both Shared Clipboard and Drag 'n' drop. This allows us to be able to copy and paste in between the host machine and the VM: <br/>
<img src="https://imgur.com/3P8uZkA.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
To increase CPU, go to System > Processor > Increase. I increased mine to 4 for speed but if you don't want this, it can be skipped <br/>
<img src="https://imgur.com/GwlepdR.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Optional: Modify network settings. I will be creating accounts using Active Directory in a separate lab, so this Server is my Domain Controller. As such, I need to have a public (NAT) and a private (box network) NIC that I could use to connect the Windows 10 VM I will be creating in another lab to my DC, and the internet. Leave Adapter 1 in its default selection. <br/>
<img src="https://imgur.com/50VYTDl.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
For Adapter 2, check Enable network adapter > Select Internal Network from the dropdown > Click OK <br/>
<img src="https://imgur.com/6T6AcUr.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
<b> Now for the VM:</b> Start VM > Click Devices > Insert Guest Additions CD Image > Go to "This PC" through File Explorer:
<img src="https://imgur.com/UrTWfYF.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Open Virtualbox Guest Additions > Double-click VBoxWindowsAdditions-amd64 and click next till you reach FInish<br/>
<img src="https://imgur.com/hpUc1Nu.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<img src="https://imgur.com/38mUzbr.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
<br />
Click Reboot Later and then shut the VM down. When you restart, you'll notice the cursor isn't lagging anymore like it was, and you can resize the window of your Server better<br/>
<img src="https://imgur.com/QmllH5H.png" height="80%" width="80%" alt="Provisioning Server 2019"/>
<br />
</p>
