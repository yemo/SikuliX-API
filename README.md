Sikuli API 1.0.1 <br />Service Update end July 2013
===========

**Download of current versions (1.0.0)** visit the official [**download page on Launchpad**](https://launchpad.net/sikuli/+download).<br />

Sikuli's Java API supporting visual testing and automation (currently using JNI/C++ to integrate with OpenCV and Tesseract)

**MANDATORY ;-)** [Have a look at major improvements and new features](https://github.com/RaiMan/SikuliX-API/wiki/Release-Notes-API)
<br /><br />
Hava a look at the Java docs: 
[click to view Online](https://dl.dropboxusercontent.com/u/42895525/SikuliX/SikuliX-API-JavaDocs/index.html)
 or [click to download as zipfile](https://dl.dropboxusercontent.com/u/42895525/SikuliX/SikuliX-API-JavaDocs.zip)


Sikuli API is targeted at people who want to develop, run and debug programs in Java, other Java based languages or Java aware scripting languages currently not supported by [Sikuli IDE](https://github.com/RaiMan/SikuliX-IDE).

Same goes for people who want to develop, run and debug scripts using Sikuli IDE supported scripting languages in other IDE's like Eclipse, Netbeans, ... [some quickstart info ...](https://github.com/RaiMan/SikuliX-API/wiki/Usage-in-Java-programming)
<br /><br />
The downloadable packages of Sikuli API contain everything needed to develop, test, run and debug with any suitable IDE (e.g. Eclipse, Netbeans, ...) or however you like ;-).
<br /><br />
This repo is **fully Maven**, so a fork of this repo can be directly used as project in NetBeans/Eclipse/... or with mvn on commandline<br /> 
It produces a lightweight **sikulix-api.jar**, that only contains the Sikuli Java API and is intended for use in pure Java or in Java aware scripting and testing environments while developing in IDEs (depends on [Sikuli Basics](https://github.com/RaiMan/SikuliX-Basics) )<br /><br />
At runtime in pure Java or in Java aware scripting and testing environments as well when using standalone Jython you need the **sikulix-java.jar** in class path (contains [Sikuli Basics](https://github.com/RaiMan/SikuliX-Basics)). <br />It can be produced using <br />*mvn -f pom_make_sikulix-java-jar.xml clean package assembly:single* <br />having a valid [Sikuli Basics](https://github.com/RaiMan/SikuliX-Basics) in your local repo.<br /><br />
To run Sikuli scripts from commandline in any of the supported scripting languages you need the **sikuli-script.jar** (currently only Jython supported).It contains [Sikuli Basics](https://github.com/RaiMan/SikuliX-Basics), [Sikuli Jython](https://github.com/RaiMan/SikuliX-Jython) and a complete Jython 2.5.4.<br />
It can be produced using <br />*mvn -f pom_make_sikuli-script-jar.xml clean package assembly:single* <br />having the mentioned dependencies in your local repo.<br />

[... click for more info](https://github.com/RaiMan/SikuliX-API/wiki/Maven-support)<br /><br />
If new to Sikuli, you might aternatively be interested in the pure Java implementation, which is to some extent feature compatible, but not API compatible: [Sikuli Java API](http://code.google.com/p/sikuli-api).
<br /><br />
**Roadmap**
 - **2013 July 6:** open a developement branch for Sikuli API 1.1
  - isolate the script running feature (already in 1.0.1) to allow more scripting languages (e.g. JRuby)
  - use existing Java wrappers for OpenCV (javacv) and Tesseract (Tes4J) alternatively
  - more enhancements tbd.
<br /><br />
 - **2013 July 29:** release of service updates Sikuli API 1.0.1
  - bug fixes and smaller enhancements 
<br /><br />
 - **2013 October 31:** release of Sikuli API 1.1
  - merge branch develop into branch master
  - open a developement branch for Sikuli API 1.2
  - new features tbd.
<br /><br />
 - **2014:** new versions in April and October

**History**
 - this is based on the developement at MIT (Tsung-Hsiang Chang (Sean aka vgod) and Tom Yeh) which was discontinued end 2011 (https://github.com/sikuli/sikuli) with a latest version called Sikuli X-1.0r930.
 - and the [follow up repo](https://github.com/RaiMan/Sikuli12.11), where I prepared the creation of a final version 1.0
 - in April 2013 I decided, to divide Sikuli into the 2 packages [Sikuli IDE](https://github.com/RaiMan/SikuliX-IDE) and Sikuli API (this repo), to better support future contributions.

**Support**
 - until otherwise noted: [questions, requests and bugs can still be posted here](https://answers.launchpad.net/sikuli)
 - the wiki in this repo will be used extensively to document anything (taking over this roll from the webpage and lauchpad)
 - you might always post an issue with any content in this repo of course

**Contribution**
 - pull requests are always welcome
 - everyone is welcome to add interesting stuff, experiences, solutions to the wiki in this repo
