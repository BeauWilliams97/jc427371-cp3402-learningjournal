# **Learning Activities & Resources**
This week I installed Wordpress on my web server.

A learning activity that I left out of last weeks journal, was installing 7zip via SSH. I used [ChatGPT](https://openai.com/chatgpt) for the install command(s). I'm glad I took the time to work this out, as it came in handy this week as well. When copying plugins/themes over to the web server, they are usually zipped to make the transfer faster, meaning that once they are copied over, they need to be unzipped/extracted. This is faster to do via SSH as opposed to doing it through FileZilla, where it can sometimes take minutes to extract. 

In relation to this, I used [How to Install a WordPress Plugin – Step by Step for Beginners](https://www.wpbeginner.com/beginners-guide/step-by-step-guide-to-install-a-wordpress-plugin-for-beginners/) & [Beginners Guide: How to Install a WordPress Theme](https://www.wpbeginner.com/beginners-guide/how-to-install-a-wordpress-theme/) to work out how to install plugins/themes manually.

I watched a bunch of YouTube videos from more experienced Wordpress Developers in order to get some sort of an insight into what the best/most useful plugins would be. I decided that for my particular startup, I would definitely need the plugins Elementor and WooCommerce. I followed along with the following tutorials to better understand both plugins:

[Elementor Wordpress Tutorial - The Basics in 10 Minutes](https://www.youtube.com/watch?v=E15iQEm9KF8) &
[How To Build An eCommerce Store in 15 Minutes](https://www.youtube.com/watch?v=zR1lpFFNwOs)

I was curious as to why numbers are used when setting directory permissions via SSH. [What Is chmod 777 and What Does It Do in Linux?](https://www.linuxscrew.com/chmod-777) More on this later in Content Insights.

I didn't migrate my site form Joomla to Wordpress this week, as I wanted to get familiar with using Wordpress and it's features. However, I did keep this in the back of my mind and researched a tutorial after I had finished the prac. [How to Easily Move Your Site from Joomla to WordPress](https://www.wpbeginner.com/wp-tutorials/how-to-move-your-site-from-joomla-to-wordpress/). This is something I will play around with during week 4. 

# **Estimated Hours & Content Insights**
I would say I spent roughly 4 hours working on this weeks content.

When installing Wordpress, it was unable to write to the config file. I had a similar issue last week when installing Joomla. I resolved it previously by setting the permission(s) for the parent directory in FileZilla and forcing all sub-directories to inheret said permissions.  

Rather than doing that again, I decided that this time around, I would work out how to give the my user write access/set directoy permissions via SSH. The following command (which was provided by ChatGPT) was used to do so: 

chmod 775 /path/to/directory

After doing some research, I discovered that the numbers (eg. 775) are used to make things quicker when assigning permissions. The first digit is "owner" permissions, the second is "group" permissions and the third is "others". 775 would give all rights to the owner, all rights groups and read and execute to others. 

Another notable thing I learned this week was that you can actually change the size of an active Azure VM. Simply click into your VM on the Microsoft Azure website, and in the left hand pane, scroll down until you see size. Click in size and you will be given a bunch of options to choose from. Simply select what size you want to re-size to, and the VM will restart. I stumbled accross this, as my web server was constantly timing out/lagging. I was being forced to restart apache every 5-10 minutes and it was hindering my work. I decided that it would be best to resize. It was likely that the cheaper option I had chosen intially didn't have good enough resources to support the web server. 

# **Career/Employability/Learning Insights**
I'm not sure how accurate this number is, but I read a statisitic online stating that 810 million websites use Wordpress, which is 43% of all the websites on the internet. [Source](https://colorlib.com/wp/wordpress-statistics/#:~:text=810%20million%20websites%20use%20WordPress%2C%20which%20is,43%25%20of%20all%20the%20websites%20on%20the%20internet).

If this is the case, learning to develop in Wordpress seems like it will definitely increase my employability. Although, I don't particularly wish to pursue front-end development. I was much more engaged when setting up the web server/back-end. 
 
