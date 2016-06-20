---
layout: post
title: Espresso 2 & OpenInEspresso
tags: [Development, Espresso, Apps, Downloads]
short-url: http://fleeting.us/pe2o
---
My development environment has long consisted of TextMate and CSSEdit. The creators of CSSEdit then released Espresso, an all-in-one app much like Coda. I tried to use it full time rather then have two apps open. However, it had some issues that kept me from using it full time. Like many I waited around for an update to CSSEdit and when [Espresso 2](http://macrabbit.com/espresso/2/) pre-release was announced I got excited. It looks like CSSEdit will no longer be a stand alone app and Espresso will take over.  This update to Espresso seems to solve any issues I had before and has some nice improvements. Looks like I might finally ditch TextMate in favor of Espresso.

There are two things in my TextMate workflow that I require with Espresso. This includes opening a file in Espresso from Terminal (quickly running `mate .gitignore` is handy) and a Finder droplet that lets me open the current window or selected file/folder in TextMate. Both of these are easy to handle. To open a file in Espresso from Terminal you need to add a new alias to your .bash_profile. In Terminal do the following:

{% highlight bash %} cd ~ open -e .bash_profile {% endhighlight %}

Add the following line to the file:

{% highlight bash %} alias esp="open -a Espresso" {% endhighlight %}

This of course requires you to reopen your terminal. Now running `esp someFile.txt` will open t hat file or folder in Espresso. Comes in very handy.

As for the OpenInEspresso Finder Droplet I modified the [OpenInTextMate](http://henrik.nyh.se/2007/10/open-in-textmate-from-leopard-finder) code to open Espresso instead. I didn't create the initial app that credit goes to Henrik Nyh for the original script. I added the Espresso icon to the bundle as I use the app icons in my finder toolbar but feel free to replace it with your icon or a Finder(ish) style button. You can drag the app to your Finder toolbar or the Finder sidebar. Clicking it will open the current window or a selected file/folder in Espresso and ready for edit.

[Download OpenInEspresso](http://downloads.monkeecreate.com/OpenInEspresso.zip)