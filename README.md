depends
=======

A tool to generate depends for repos. Similar to google depot_tools, but without rietveld,
and much simpler


Problems
========

* Too many repos
* A repo depends on B repo on special version
* A repo requires B repo in a special directory for compiling or testing...
* B repo is used by A and C repo ...


Solutions
=========

* A tool to automatically put the repos you want in a relative directory you want!
* Can specify version
* Can work with git svn
* Can support diff  
* If possible with some sort of posibilities to extend.


Usage
=====

Create a new Structure for your project.
----------------------------------------
root	           
>.depends---This file will be created by the depends tool	
>repo           
>>include
>>src	   
>>DEPS---This file should be created by yourself

A simple way to start.
----------------------

* mkdir NewProject
* git clone https://github.com/sloanyang/depends.git
* ./depends/depends config your repo (For Example: https://github.com/sloanyang/aquantic.git)
* Well Done :)
