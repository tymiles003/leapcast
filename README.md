# leapcast
[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=dz0ny&url=https://github.com/dz0ny/leapcast&title=Leapcast&language=&tags=github&category=software)
[![Build Status](https://travis-ci.org/dz0ny/leapcast.png?branch=master)](https://travis-ci.org/dz0ny/leapcast)


Simple ChromeCast emulation app.

Working:

 - Discovery (DIAL protocol http://www.dial-multiscreen.org/)
 - Youtube (with https://play.google.com/store/apps/details?id=com.google.android.youtube)
 - Google Music (with https://play.google.com/store/apps/details?id=com.google.android.music)
 - HBO GO (with https://play.google.com/store/apps/details?id=com.HBO)
 - Hulu Plus (with https://play.google.com/store/apps/details?id=com.hulu.plus)
 - Pandora (with https://play.google.com/store/apps/details?id=com.pandora.android )
 - RedBull TV (with https://play.google.com/store/apps/details?id=com.nousguide.android.rbtv)
 - Others (see http://en.wikipedia.org/wiki/Chromecast#Chrome_and_mobile_apps)
 
On real device enabled apps are fetched from https://clients3.google.com/cast/chromecast/device/config .
Bugs in ChromeCast SDK are listed at https://code.google.com/p/google-cast-sdk/issues/list?can=2&q=&sort=priority&colspec=ID%20Type%20Status%20Priority%20Milestone%20Owner%20Summary 

Some known bugs in ChromeCast SDK:
 
 - Discovery fails on some devices with multiple unactive network interfaces 
 - Scanning crashes device or app with ConcurrentModificationException 

## Authors

The following persons have contributed to leapcast.

 - Janez Troha
 - Tyler Hall
 - Edward Shaw
 - Jan Henrik
 - Martin Polden
 - Thomas Taschauer
 - Zenobius Jiricek
 - Ernes Durakovic
 - Peter Sanford
 - Michel Tu

## How to install

### Simple

Clone this directory, then run ```python setup.py develop``` or ```pip install leapcast```

### Better

```
git clone https://github.com/dz0ny/leapcast.git
cd ./leapcast
sudo apt-get install virtualenvwrapper python-pip python-twisted-web python2.7-dev
mkvirtualenv leapcast
pip install .
```

#### Windows

For those on Windows(tm) follow this guide https://gist.github.com/eyecatchup/6219118 or https://plus.google.com/100317092290545434762/posts/8RjWfMXxje8

```
usage: leapcast [-h] [-d] [--name NAME] [--user_agent USER_AGENT]
                [--chrome CHROME] [--fullscreen]

optional arguments:
  -h, --help            show this help message and exit
  -d                    Debug
  --name NAME           Friendly name for this device
  --user_agent USER_AGENT
                        Custom user agent
  --chrome CHROME       Path to Google Chrome executable
  --fullscreen          Start in full-screen mode
  --window_size         Force the initial window size (eg 1920,1080)

```


[![Bitdeli Badge](https://piwik-ubuntusi.rhcloud.com/piwik.php?idsite=2&amp;rec=1)](https://bitdeli.com/free "Bitdeli Badge")

