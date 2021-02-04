# Raspbian:

How did you install your Version of Hyperion?

* [I downloaded a .deb package and installed it via `apt` or `dpkg`](/txt/raspbian.md#pick-your-system)

&nbsp;

* [I compiled it via CompileHowto.md, but did not use docker.](/txt/compile.md#Updating-a-compiled-version-of-hyperion) 


&nbsp;

* I made a [docker](https://github.com/hyperion-project/hyperion.ng/blob/master/CompileHowto.md#with-docker) container ---N/A

<a href="https://github.com/hyperion-project/hyperion.ng"><img src="/pictures/logo.png" width="350" alt="github hyperion logo"></a>


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

# Pick your System:

* [I use a Raspberry Pi 1 or Zero](/txt/raspbian.md#deb-package-pi-10)

* [I use a Raspberry Pi 2/3/4](/txt/raspbian.md#deb-package-pi-234)

<a href="https://github.com/hyperion-project/hyperion.ng"><img src="/pictures/logo.png" width="350" alt="github hyperion logo"></a>


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

Now we remove the old package, you can skip this:
<pre><code>sudo apt remove hyperion</code></pre>

Choose Package

You can find the latest packages on the Release page. You can copy the file from the "Assets" Dropdown Menu. The Pi 1/0 needs an `armv6l.deb`. I will use the Alpha.7 release as an example.

Download
<pre><code>wget https://github.com/hyperion-project/hyperion.ng/releases/download/2.0.0-alpha.7/Hyperion-2.0.0-alpha.7-Linux-armv6l.deb</code></pre>

Installation
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

Now we remove the old package, you can skip this:
<pre><code>sudo apt remove hyperion</code></pre>

Choose Package

You can find the latest packages on the Release page. You can copy the file from the "Assets" Dropdown Menu. The Pi 2/3/4 needs an `armv7l.deb`. I will use the Alpha.7 release as an example.

Download
<pre><code>wget https://github.com/hyperion-project/hyperion.ng/releases/download/2.0.0-alpha.7/Hyperion-2.0.0-alpha.7-Linux-armv7l.deb</code></pre>

Installation
<pre><code>sudo apt install ./Hyperion-2.0.0-alpha.7-Linux-armv7l.deb</code></pre>

Checking for missing dependencies
<pre><code>sudo apt -f install</code></pre>

Now reboot... 

Does the GUI/Webinterface work?  [Yes](/txt/congratulation.md#Congratulations) / [No](/txt/service.md#checking-for-a-working-installation) 


&nbsp;


&nbsp;


&nbsp;


&nbsp;
