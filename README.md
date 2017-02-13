# RaspberryPiSplash
Custom Splash Screen for Raspberry Pi (Raspbian or ChromePi)

This is a quick and dirty solution for an unanimated custom splash screen during boot.
<ol>
<li>Update you Raspberry Pi with the latest update
<ul>
<li>sudo apt-get -y update</li>
<li>sudo apt-get -y upgrade</li>
</ul>
<li>Install fbi which can show image in full screen in console mode.</li>
<ul>
<li>apt-get install -y fbi</li>
</ul>
<li>Copy your custom splash image to /home/pi and name it "splash.png".
<li>Copy asplashscreen script to "/etc/init.d" folder

<li>Make the script executable and create a service for init mode so that asplashscreen will run at boot</li>
<ul>
<li>chmod a+x /etc/init.d/asplashscreen</li>
<li>insserv /etc/init.d/asplashscreen</li>
</ul>
<li>Reboot and watch your custom splash screen come to action.
<br>
<br>
Alternatively you can run the below command which will run the script from this repository and create and copy all the above to your respective folder.
At your prompt type
