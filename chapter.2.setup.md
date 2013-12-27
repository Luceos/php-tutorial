# Set up your development
> The best way to learn, is by doing

In order for you to start building your first web application you will need a development environment. We will start quickly if you follow the steps for your preferred platform. Once you followed the tutorial you will have made your current PC into a webserver. A local webserver allows for rapid development and testing.

Please select the operating system you are working on right now to install the necessary software to turn your local system into a webserver. If you rather prefer to keep your PC clean or you don't know how to start, just ask your mentor for a remote webhosting package.

### Windows

Install [wampserver.com](http://www.wampserver.com/en/#wampserver-64-bits-apache-2-4).

### Mac

Follow this [tutorial by Jason McCreary](http://jason.pureconcepts.net/2012/10/install-apache-php-mysql-mac-os-x/).

### Ubuntu

Follow this [tutorial by Digital Ocean](https://www.digitalocean.com/community/articles/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu).

## Your webserver

You now have made a local [webserver](http://en.wikipedia.org/wiki/Webserver). Webservers are computers, like yours, which are placed in a building (called [datacenter](http://en.wikipedia.org/wiki/Data_center)) with a fast internet connection and other, for hosting, benefits.

### Anatomy of a webserver

The webserver you now are running on your machine uses the software Apache, just like Microsoft Word, Apache is responsible for serving pages to a visitor. The default input it asks for is HTML. However you also installed PHP, which allows for dynamic functionality.

### Serving code

Webservers are optimized to serve code to it's visitors, this can be any markup or programming language supported by the webserver. Your own local machine now also serves code. Just visit http://localhost or http://127.0.0.1 to visit your current default webpage.

### Application states

In development we talk about several development stages. The first being development, where developers built, change and fix applications. The second being a testing environment where changes are tested. The third is the staging environment where customers can test out and give feedback on features or fixes. The last one is production, which is the live website.

Not all companies keep to these 4 stages, but trying to adhere to them often increases the stability of the production environment. Production environments most often do not run on the same machine (webserver) as the other stages, because technical complications might create disruptions in the production environment.

### Why hosting your production website locally is unwise

We have set up a webserver on your local machine now. Once you've mastered the basics of webdevelopment and have a website which you'd like to have online permantly I advise you to get some real webhosting; your mentor will have some preferred partners for that. If not, just take a look at [HostingXS](http://www.hostingxs.com).

It's unwise to run production websites on your local machine or even at home. Although many homes are equipped with fiber internet, your equipment and connection can never match those of a datacenter.