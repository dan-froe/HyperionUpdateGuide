# Updating LibreELEC! 

###### [credits to Paulchen-Panther\'s guide](https://hyperion-project.org/threads/install-hyperion-ng-on-libreelec-x86_64-rpi-inoffiziell-unofficially.10463/) 


First of all we deinstall the Addon via ssh

<pre><code>systemctl disable hyperion.service --now
rm -R /storage/hyperion</code></pre>

Now we use the following script
<pre><code>wget -qO- https://git.io/JU4Zx | bash</code></pre>
