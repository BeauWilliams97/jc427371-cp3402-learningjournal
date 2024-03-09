# **Learning Activities & Resources**
This week I used VVV to set up a dynamic site with a database running on my localhost.

[VVV Documentation](https://varyingvagrantvagrants.org/) - I used this guide to understand how to set up VVV via CLI. I also used the videos provided on LearnJCU.

Something I believe I learnt/developed during this weeks practical exercise, was a basic understanding of how Vagrant utilizes virtualisation to create isolated development environments. From my understanding, Vagrant leverages some sort of virtualisation software such as Virtual Box, VMWare, etc. to create an isolated virtual machine(s) on the users local system. Said VMs simulate a complete computing environment, including an operating system, storage and networking resources. 

At the heart of all of this, is Vagrant's configuration file - Vagrantfile. The file is written in Ruby and defines a lot of the stuff previously mentioned, such as the characteristics of the VM(s) networking settings, provisioners, the box image used, etc. 

I also learnt a little bit about Vagrant CLI and the basic commands needed to interact with/manage virtual environments created. Some of these commands include 'vagrant up' (which starts the VM), 'vagrant halt' (which stops the VM), 'vagrant reload' (reload VM/apply changes to Vagrantfile), and 'vagrant destroy' (used to delete the VM).

# **Estimated Hours & Content Insights**
I spent roughly 2 hours working on this practical. Very little time spent was this week as the entire process has been thoroughly explained on LearnJCU. 

Initially, I had some issues with being able to access the sites provisioned by VVV(vvv.test, one.wordpress.test, etc.). I believe VVV was unable to write to my hosts file because anti-virus software installed on my machine was preventing it. This was surprising to me, and something I had not anticipated. 

I quickly uninstalled said software and ran 'vagrant up --provision' and it resolved the issue. Prior to uninstalling the software, I had tried to add vvv.test, etc. to the hosts file manually but was unable to save the file after making changes. In relation to this problem, I learned which directory the Windows hosts file is located in, how to edit it, and also the purpose that it serves.

Provided there isn't some sort of software preventing it, changes to the host file can be made by launching notepad in administrator, or by navigating to C:\Windows\System32\drivers\etc via CLI and typing 'notepad hosts'. This will then open the file in an administrator version of notepad and will allow you to make the desired changes. 

# **Career/Employability/Learning Insights**
If I was planning on pursuing a career in web development, knowing how to set up Vagrant/Virtualy Box/VVV would be very useful. In hindsight, I wish I used VVV for the majority of my A1 development, and created the live server only once I was prepared to push to production. This would have saved money on hosting and also would have helped me avoid issues/prevent server bloating created from faulty Joomla plugins, as I would know what to avoid installing/doing when dealing with the live server. 
 
