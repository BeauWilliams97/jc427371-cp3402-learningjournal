**Learning Activities & Resources**
This week I made a another website. However, this time I used the CMS framework Joomla. I also changed hosting providers. Instead of using Github Pages, I used Micrsoft Azure. 

Unfortunately, I don't have links to all of the resources I used this week to complete the practical. From memory, there is definitely some stuff I wasn't able to track down again. 

I followed [this](https://www.youtube.com/watch?v=p4aXonUEeQ4) to get MySQL, php, and phpMyAdmin installed on the web server. This tutorial also helped me understand how to set the neccessary permissions for my user to create a db. 

I used [this](https://www.youtube.com/watch?v=ccwzg_F76tk) to work out how to customise the CSS of my Joomla site. I wanted to change the colour of the header and footer. I also wanted to use CSS to turn off the annoying display information attached to every article upon creation. 

I used [this](https://www.youtube.com/watch?v=PmAKzOBLp4U) to work out how to add functionality to the buttons in the navbar. 

**Estimated Hours & Content Insights**
I would say I spent less time working on the pracitcal this week than I did last week. Probably roughly 5 hours. The most time consuming part was creating the web server and getting all of the neccessary prerequistes installed. 

I made a web server in AWS last semester for Cloud Computing, so I was somewhat familar with the process already. I managed to create a VM and install apache2, php, phpmyadmin and MySQL pretty quickly and without too much resistance. I used PuTTYgen to convert the .pem file (supplied by Azure when the VM is created) to a .pk file which I then used to SSH into the web server. I also used PuTTY for this. 

After I was confident I had all of the neccessary prerequisites installed and that the web server was up and running, I transferred the Joomla files over via SFTP using FileZilla. 

When I tried to install Joomla, I was met with an error saying that the version of php I had installed needed to be updated to 8.1 (I think it was 7.4 or something initally). For some reason, updating php took a good amount of my time haha. At least an hour. I couldn't seem to find the right command(s). I was also unaware that you needed to dismod the previous version and enmod the updated version for it to work after installation. I think one of the comments on [this](https://askubuntu.com/questions/1373755/how-to-change-php-version-in-ubuntu-20-04-console) forum made me aware of that. 

Once php was updated, I immediately ran into another error - Joomla was saying that the autoload_psr4.php file wasn't being created. I managed to resolve this by changing the file permissions for the joomla folder in FileZilla, and then setting the administrator folder, and all files within, to inheret permissions from the parent directory. 

It was pretty much smooth sailing from there.

**Career/Employability/Learning Insights**
I don't think knowledge of Joomla will ever benefit me in the future haha. I wouldn't use it again. It was more annoying than anything. 

I think a lot of the general knowledge that comes with actually being able to create a web server is useful. Also, understanding what components it needs to operate and why etc. is also a big take away from this weeks content, in my opinion. 

Using PuTTY and FileZilla is undoubtedly something I will need to do again, and getting familair with how they both work was cool and something I enjoyed. 
