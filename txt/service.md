# Checking for a working installation!

Does the GUI work after typing `hyperiond` in the SSH?

[Yes](/txt/service.md#you-are-missing-configurations) / [No](/txt/bad.md#something-went-wrong-probably)


&nbsp;


&nbsp;

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

### You are missing configurations!

Please edit the following files and change them accordingly. It is probably just `User=pi` in the first file. 

<pre><code>sudo nano /etc/systemd/system/multi-user.target.wants/hyperiond@pi.service</code></pre>

<pre><code>[Unit]
Description=Hyperion ambient light systemd service  for user %i
After=network.target

[Service]
ExecStart=/usr/bin/hyperiond
WorkingDirectory=/usr/share/hyperion/bin
User=pi
TimeoutStopSec=5
KillMode=mixed
Restart=on-failure
RestartSec=2

[Install]
WantedBy=multi-user.target</code></pre>

Next file:

<pre><code>sudo nano /etc/systemd/system/hyperiond@.service</code></pre>

<pre><code>[Unit]
Description=Hyperion ambient light systemd service  for user %i
After=network.target

[Service]
ExecStart=/usr/bin/hyperiond
WorkingDirectory=/usr/share/hyperion/bin
User=%i
TimeoutStopSec=5
KillMode=mixed
Restart=on-failure
RestartSec=2

[Install]
WantedBy=multi-user.target</code></pre>


&nbsp;
Now we are restart the process:

<pre><code>sudo systemctl daemon-reload
sudo systemctl enable hyperiond@pi.service
sudo systemctl start hyperiond@pi.service</code></pre>
