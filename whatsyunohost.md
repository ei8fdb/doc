What is YunoHost?
=================

<img src="/images/YunoHost_logo_vertical.png" width=400>

YunoHost is an **operating system** aiming to simplify as much as possibly the administration of a **server** and therefore democratize [self-hosting](selfhosting), while making sure it stays reliable, secure, ethical and lightweight. It is a free software project maintained exclusively by volunteers. Technically, it can be seen as a distribution based on [Debian GNU/Linux](https://debian.org) and can be installed on [many kinds of hardware](install).

Features
--------

- <img src="/images/icon-debian.png" width=32 style="margin-right:5px"> based on Debian ;
- <img src="/images/icon-tools.png" width=32 style="margin-right:5px" width=64> administrate your server through a **friendly web interface** ;
- <img src="/images/icon-package.png" width=32 style="margin-right:5px"> deploy **applications in just a few clicks** ;
- <img src="/images/icon-users.png" width=32 style="margin-right:5px"> manage **users** <small>(based on LDAP)</small>;
- <img src="/images/icon-globe.png" width=32 style="margin-right:5px"> manage **domain names** ;
- <img src="/images/icon-medic.png" width=32 style="margin-right:5px"> create and restore **backups** ;
- <img src="/images/icon-door.png" width=32 style="margin-right:5px"> connect to all apps simultaneously through the **user portal** <small>(nginx, SSOwat)</small> ;
- <img src="/images/icon-mail.png" width=32 style="margin-right:5px"> includes a **full email stack** <small>(Postfix, Dovecot, Rspamd, DKIM)</small> ;
- <img src="/images/icon-messaging.png" width=32 style="margin-right:5px"> ... as well as **an instant messaging server** <small>(XMPP)</small> ;
- <img src="/images/icon-lock.png" width=32 style="margin-right:5px"> manages **SSL certificates** <small>(based on Let's Encrypt)</small> ;
- <img src="/images/icon-shield.png" width=32 style="margin-right:5px"> ... and **security systems** <small>(fail2ban, yunohost-firewall)</small> ;

Origin
------

YunoHost was created in February 2012 after something like this:

 <blockquote><p>"Shit, I'm too lazy to reconfigure my mail server... Beudbeud, how were you able to get your little server running with LDAP?"</p>
<small>Kload, February 2012</small></blockquote>

All that was needed was an administration interface for Beudbeud's server to make something usable, so Kload decided to develop one. Finally, after automating several configurations and packaging in some web apps, YunoHost v1 was finished.

Noting the growing enthusiasm around YunoHost and around self-hosting in general, the original developers along with new contributors decided to start work on version 2, more extensible, more powerful, more easy-to-use, and one that makes a nice cup of fair-trade coffee for the elves of Lapland.

The name **YunoHost** comes from the jargon "Y U NO Host". The [Internet meme](https://en.wikipedia.org/wiki/Internet_meme) should illustrate it:
<div class="text-center"><img style="border-radius: 5px; box-shadow: 0 5px 15px rgba(0,0,0,0.15);" src="/images/dude_yunohost.jpg"></div>

What YunoHost is not?
---------------------

Even if YunoHost can handle multiple domains and multiple users, it is **not meant to be a mutualized system**.

First, the software is too young, not tested at large scale and thus probably not optimized to be put in production for hundreds of users at the same time. With that said, we do not want to lead the software in that direction. Virtualization democratizes, and its usage is recommended since it is a more leaktight way to achieve mutualization than a "full-stack" system like YunoHost.

You can host your friends, your family and your company safely and with ease, but you must **trust your users**, and they must trust you above all. If you do want to provide YunoHost services for unknown persons anyway, a full VPS per user will be just fine, and we believe is a better way to go.

Art Works
---------

Black and white YunoHost png logo done by ToZz (400 × 400 px):

<a href="/images/ynh_logo_black_300dpi.png"><img src="/images/ynh_logo_black_300dpi.png" width=220></a>

<a href="/images/ynh_logo_white_300dpi.png"><img src="/images/ynh_logo_white_300dpi.png" width=220></a>

Click to download.

Licence: CC-BY-SA 4.0
