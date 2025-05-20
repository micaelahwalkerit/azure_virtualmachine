# azure_virtualmachine
<p align="center">
<img src="https://i.imgur.com/JRnq4PQ.png" alt="Microsoft Azure Logo"/>

</p>

<h1>Creating a Virtual Machine (Azure)</h1>
This tutorial outlines how to create a Virtual Machine within Microsoft Azure. </br>
</br>
<i> What is a Virtual Machine? </i> A virtual machine is a computer created using software that runs inside your main physical computer. It’s like having a second, separate computer within your existing one, made possible by tools like Microsoft Azure. Each virtual machine works on its own, with its own system, programs, and files—just like a real computer. Using a virtual machine in Azure makes it easy to run different systems  (OS systems), save money on hardware, and safely test software in a secure environment (a.k.a "The Cloud).
<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)



<h2>Operating Systems Used </h2>

- Windows 10 Pro, version 22H2 - x64 Gen2 <b>(example for VM set-up)</b>

<h2>Prerequisites</h2>

- Create an Azure Account (Tenant (Organization) and Subscription)
- Sign into Azure Account

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1 - Create a Resource Group 
- Step 2 - Create a Virtual Machine
- Step 3 - Fill in the Basics Tab
- Step 4 - Disk Tab
- Step 5 - Networking Tab (Create Virtual Network & Subnet)
- Step 6 - Monitoring/Management Tab
- Step 7 - Review + Create ( Virtual Machine )
- Step 8 - Deployment
- Step 9 - Check to see if Virtual Machine is Successfully Running &#128077; &#x1F604;

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/TaeIVwZ.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>


<b> **PRE-STEP** -- After signing in to Azure, click on "Resource Groups" in the dashboard. You will be redirected to the "Create Resource Group" page.</b>
</p>
<br />
<br />
<br />



<p>
<img src= "https://i.imgur.com/qB68NYR.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>

<h3><b> Step 1 - Create a Resource Group </b></h3>
  
<p>Make sure that the resource group is created under the correct <b>Subscription.</b>

Next, enter a <b>Resource Group Name</b> that is easy to recognize and will be used to contain your Virtual Machine.

Next, select a <b>Region</b> that is geographically close to your location for optimal performance.

Finally, click <b>Review + Create</b> to create the Resource Group
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/DVnMCCU.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>
<p>
<h3><b> Step 2 - Create a Virtual Machine</b></h3>
  <br />

After creating your resource group, return to the Azure Dashboard.

Next, click on <b>"Virtual Machines" </b>— you can find this either on the dashboard or in the left-hand navigation menu.

Then, click the <b>"+ Create"</b> button and select <b>"Azure virtual machine"</b> from the dropdown.
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/aST7Tc3.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>
<p>
<h3><b>Step 3 - Fill in Basic Tab for your Virtual Machine </b></h3>
<br />
  
After clicking <b>"Azure virtual machine"</b> from the dropdown menu, you'll be taken to the <b>Basics</b> tab. This is where you'll enter the essential information needed to set up your virtual machine.

<b>Fill in the following fields:</b>

<b>Subscription:</b> Select the appropriate subscription from the list.

<b>Resource Group:</b> Choose the resource group you created earlier.

<b>Virtual Machine Name:</b> Enter a name for your VM (e.g., MyFirstVM).

<b>Region:</b> Select the same region you used for your resource group.

<b>Image:</b> Choose the operating system you'd like to install (e.g., Windows 11, Ubuntu).

<b>Size:</b> Click "See all sizes" and select a VM size that fits your performance needs and budget. (However, it's best to choose at least 2 vcpus for speed)

<b>Administrator Account Setup:</b>

<b>Username:</b> Create a secure username for logging into your VM.

<b>Authentication Type:</b>

<ul>For <i>Windows</i>, set a strong password.

For <i>Linux</i>, upload an SSH public key or choose password authentication if preferred. ( Azure now automatically generates an SSH key pair for you but you can also just use a Username & Password like you would for Windows).</ul>

<b>Licensing:</b> (Usually for a Windows VM) If you see a Licensing checkbox, check it or else your VM will fail to deploy.

Click <b>"Next: Disk"</b>
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/c9ucNHD.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>
<p>
<h3><b>Step 4 - Disks Tab </b></h3>
<br />

Leave defaults (or choose SSD for better performance).

Click <b>"Next: Networking"</b>.
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/IWOHYJU.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>
<p>
<h3><b>Step 5 - Networking Tab</b></h3> 
  <br />

Azure will automatically create a <b>Virtual Network (VNet) and Subnet</b>. However, you can change the VNet name.
<br />
<ul><i>This is one of Azure's helpful features for a virtual machine. These are essential because they allow your VM to communicate with other resources, just like a physical computer on a network</i></ul>

Ensure <b>"Public IP"</b> is set to create a new one (if you want internet access).

<b>Leave defaults unless you have specific networking needs.</b>
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/s6te31Q.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>
<p>
<h3><b> Step 6 - Management, Montoring, Advanced,Tag Tabs </b></h3>
  <br />
This step is pretty easy! You can leave the options as they are! Wahoo, this is last aspect of "set-up" &#129395;
<br />
Click <b>Review + Create<b/>
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/YBEt0H5.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>
<p>
<h3><b>Step 7 - Review + Create</b></h3>
<br />


Wait for validation to pass.

Click <b>"Create."</b>
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/DTPz4WR.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>
<p>
<h3><b>Step 8 - Wait for Deployment to Take Place</b></h3>
<br />
  
Azure will take a few minutes to create your Virtual Machine based on all of the configurations from the previous steps.

Once done, click "Go to resource" to view your new virtual machine and observe VNet and Subnet to make sure it matches what was configured in previous steps.
</p>
<br />
<br />
<br />
<br />

<p>
<img src="https://i.imgur.com/NdZHP4m.png" height="80%" width="80%" alt="Azure Virtual Machine Steps"/>
</p>

<h3><b>Step 9 - Check to see if Virtual Machine is Successfully Running</b></h3>
<br />
 <p>
Click <b> "Home".</b>

Click <b>"Virtual Machines".</b>

See if the Virtual Machine you created is running
</p>
<br />
<br />
<br />
<br />

<h2>In Conclusion</h2>
<p>
Creating a virtual machine in Azure lets you run a computer in the cloud for tasks like running apps, storing data, or testing software. It’s a fast and flexible way for businesses to build secure infrastructure, protect their data, and manage systems without needing physical equipment. Learning how to set up a virtual machine helps both individuals and organizations work more efficiently and safely in the cloud.
</p>





