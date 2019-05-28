# DAIWSI
Downloading Anything Of the Internet Without Searching It.

This setup helps you download anything off the internet without even searching for it.

We're gonna setup our SABnzbd++ to download webseries and its upcoming episodes without user interaction. Hence Automating the whole process of searching and downloading.

**Before Usage Dependencies Required -**
	

## **Setup SABnzbd**

    sudo apt-get install software-properties-common

    sudo add-apt-repository multiverse

    sudo add-apt-repository universe

    sudo add-apt-repository ppa:jcfp/nobetas

    sudo add-apt-repository ppa:jcfp/sab-addons
    sudo apt-get update && sudo apt-get dist-upgrade
    sudo apt-get install sabnzbdplus python-sabyenc

    sudo apt-get install par2-tbb

**Start SABNzbdplus**

> sabnzbdplus

or
 

this will open a tab on [http://localhost:8080](http://localhost:8080)



## User Accounts needed

 - https://free-usenet.com/login/
 
Go to Free Account tab and copy the credentials and use them to login to [http://localhost:8080](http://localhost:8080)
After Logging in,
 - click _Config_. Beneath _Config_, click _General_. First you'll find the configuration for the SABnzbd web server. Set bandwidth limit to 1Mbps
 - In the last config sub-category, _Sorting_, you can do some pretty neat things with the organization of your downloads. There are a couple of sorting options, You can use this to sort episodes however you'd like. Here's one example:

> Sort string:  
> %sn - Episode %s%0e - %en.%ext
> 
> Output:  
> Show Name - Episode 105 - Episode Name.avi

Now that you've set up SAB, it's time to give it something to download. SAB downloads and processes files via NZBs.

**Head over to
https://www.nzbindex.com/search**

We'll find RSS feed of our favorite series, movies or any packages that we need to download.

 1. Search for any show or webseries
 2. Click on the RSS Feed option, you'll be redirected to a new tab containing XML version 
 3. Copy the URL of the new tab and headover to your local host at port 8080 and add a new RSS url with the url you copied
 4. Leave and Enjoy

