WebSockit2me is a WebSocket to TCP gateway built on TclHttpd for both noVNC and the WebSocket Telnet Client.It provides a similar function to the Python Package "Websockify" except it's built into a web server with noVNC preloaded.

TclHttpd is a pure Tcl implementation of a Web server. WebSockit2me is packaged for easy deployment as a Starkit. Just download 2 files and you're ready to go. To uninstall just delete the 2 files.

Some of the features include:

    Access Control for multiple users to the WebSocket to TCP gateway via Basic Authentication using an Apache-style htpasswd file. This file can be generated by an external program or the built in Access Control Editor.

    HTTPS(SSL) support built in using the Tcl TLS (1.6.8) extension for Linux 32/64, Windows 32/64 and Mac OSX.

    noVNC v1.2.0 included with the ability to upgrade to a later version.

    WebSocket Telnet Client included.

    Dynamically set the Host and Port you wish to establish a connection with. This feature is only accessible with Authentication.

    Statically set the Host and Port via a Target File ("whitelist") using "tokens" in the Url query parameters to select the correct Host and Port to connect too. This feature can be accessed with or without Authentication. 

Uses:

    Run on the same box that has a VNC/Telnet Server loaded so it can be accessed via a modern web browser.

    Run on a central box to access multiple remote VNC Servers and Telnet Servers via a modern web browser.

    (web browsers must be capable of supporting WebSockets see Browser Support ) 

Try it Out

Click on the "Dynamic" link at the bottom of the page and type in the Host and Port of the VNC or Telnet Server you wish to connect with. The webmaster username and password will work.

Click on the Static link at the bottom of the page to connect with a VNC Server on this machine. (You need to have VNC server running on the default port of 5900 and allow connections from the loopback or localhost.) If this browser is running on the same machine as the VNC Server you will experience a cascading window effect. Try it from a remote machine to display the correct desktop.

Quick Start Guide

    Download the Tclkit suitable for your platform from Tclkit Downloads page. http://tclkits.rkeene.org/fossil/wiki/Downloads
    Download the WebSockit2me Starkit. 
    Create a directory for example

    C:\WebSockit2me

    or

    /usr/local/websockit2me

    and place the Tclkit and WebSockit2me.kit files in that directory.

    On Linux

    chmod +x tclkit (rename the downloaded tclkit file to something shorter if desired eg tclkit-8.6.3)

    ./tclkit-8.6.3 WebSockit2me.kit

    On Windows

    Rename the downloaded tclkit file to something shorter if desired and include ".exe" on the end eg tclkit-8.6.3.exe

    from a DOS prompt:

    tclkit-8.6.3.exe WebSockit2me.kit

    from File Explorer:

    drag WebSockit2me.kit over tclkit-8.6.3.exe and release 

Point your browser to http://Your-IP-Address:8015/

Important

    If you plan to access over the Internet, check the FAQ and only access via HTTPS. Also enable Authentication!
    The default password for webmaster is webmaster. Please change this ASAP via the Access Control Editor. 

Licenses

    WebSockit2me and TclHttpd are distributed under a copyright that allows free use.
    noVNC and the WebSocket Telnet Client are under various Licenses listed in the /kanaka directory. 

This project is tested with BrowserStack.

<!--
**WebSockit2me/Websockit2me** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
