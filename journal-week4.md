# **Learning Activities & Resources**
This week I used VVV to set up a dynamic site with a database running on my localhost.

[VVV Documentation](https://varyingvagrantvagrants.org/) - I used this guide to understand how to set up VVV via CLI. I also used the videos provided on LearnJCU.

# **Estimated Hours & Content Insights**
I spent roughly 2 hours working on this practical. Very little time was this week as the entire process has been thoroughly explained on LearnJCU. 

Initially, I had some issues with being able to access the sites provisioned by VVV (vvv.test, one.wordpress.test, etc.). I believe VVV was unable to write to the hosts file because my anti-virus software was preventing it. I uninstalled said software and ran vagrant up --provision, and it resolved the issue. Prior to uninstalling the software, I had tried to add vvv.test, etc. to the hosts file manually but was also unable to save the file after making changes. In relation to this problem, I learned which directory the Windows hosts file is located in, how to edit it, and also the purpose that it serves.

Provided there isn't some sort of software preventing it, changes to the host file can be made by launching notepad in administrator, or by navigating to C:\Windows\System32\drivers\etc via CLI and typing 'notepad hosts'. This will then open the file in notepad and allow you to make the desired changes. 

# **Career/Employability/Learning Insights**
If I was planning on pursuing a career in web development, knowing how to set up VVV would be very useful. In hindsight, I wish I used VVV for the majority of my A1 development, and created the live server only once I was prepared to push to production. This would have saved money on hosting and also would have helped me avoid issues/prevent server bloating created from faulty Joomla plugins as I would know what to avoid installing on when dealing with the live server. 
 
