# Pick your System:

* [I use a Raspberry Pi 1 or Zero](/txt/hyperbian.md#deb-package-pi-10)

* [I use a Raspberry Pi 2/3/4](/txt/hyperbian.md#deb-package-pi-234)


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;
&nbsp;


&nbsp;


&nbsp;


&nbsp;


## .deb Package Pi 1/0

First of all, we update the System
<pre><code>sudo update
sudo full-upgrade</code></pre>

#### Choose Package

You can find the latest packages on the Release page. You can copy the file from the "Assets" Dropdown Menu. The Pi 1/0 needs an `armv6l.deb`. I will use the Alpha.7 release as an example.

#### Download
<pre><code>wget https://github.com/hyperion-project/hyperion.ng/releases/download/2.0.0-alpha.7/Hyperion-2.0.0-alpha.7-Linux-armv6l.deb</code></pre>

### Installation
<pre><code>sudo apt install ./Hyperion-2.0.0-alpha.7-Linux-armv6l.deb</code></pre>

Checking for missing dependencies
<pre><code>sudo apt -f install</code></pre>

Now reboot

Does the GUI/Webinterface work?  [Yes](/txt/congratulation.md#Congratulations) / [No](/txt/service.md#checking-for-a-working-installation) 



&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


## .deb Package Pi 2/3/4

First of all, we update the System
<pre><code>sudo update
sudo full-upgrade</code></pre>

#### Choose Package

You can find the latest packages on the Release page. You can copy the file from the "Assets" Dropdown Menu. The Pi 2/3/4 needs an `armv7l.deb`. I will use the Alpha.7 release as an example.

#### Download
<pre><code>wget https://github.com/hyperion-project/hyperion.ng/releases/download/2.0.0-alpha.7/Hyperion-2.0.0-alpha.7-Linux-armv7l.deb</code></pre>

#### Installation
<pre><code>sudo apt install ./Hyperion-2.0.0-alpha.7-Linux-armv7l.deb</code></pre>

Checking for missing dependencies
<pre><code>sudo apt -f install</code></pre>

Now reboot... 

Does the GUI/Webinterface work?  [Yes](/txt/congratulation.md#Congratulations) / [No](/txt/service.md#checking-for-a-working-installation) 


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;


&nbsp;
# Hyperbian 

HyperBian is Raspbian with the newest version of hyperion pre-installed. 
You will have to write a new image on your SD card. 

* Backup up your configuration in Hyperion. 

* Download [HyperBian](https://github.com/hyperion-project/hyperion.ng) and flash it on your SD card. 

* Import your backup configuration into [hyperion](http://HyperBian:8090). 



