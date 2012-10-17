CMUSphinx Long Audio Aligner
----------------------------

AUTHORS			  
-------
* Bhiksha Raj 		  : CMUSphinx Mentor GSoC 2011
* Nickolay Shymrev 	: CMUSphinx Mentor GSoC 2011
* James Baker 		  : CMUSphinx Advisor GSoC 2011
* Antony Robinson		: CMUSphinx Advisor GSoC 2011
* Rita			        : CMUSphinx Advisor GSoC 2011

* Apurv Tiwari		  : Student GSoC 2011 

ABOUT
-----
Speech and text alignment finds applications in fields such as multimedia indexing 
and training of large vocabulary speech recognition. This project is designed to provide
this functionality in CMUSphinx's Sphinx4 decoder.

Result of a typical audio - text alignment is a sequence of word indexed with their start
and end time in the audio.

REQUIREMENTS
------------
i) JDK version >= 1.6.x.x
ii) Sphinx4.jar 

RUN INSTRUCTIONS
----------------
To run the demo :

i) Build the program by issuing

    $ ant all

This will give you `bin/aligner.jar`

ii) Run it by doing

    $ java -ms400m -mx1500m -jar bin/aligner.jar <path-to-audio-file> <path-to-transcript-file>

UNDERSTANDING THE RESULT OF ALIGNMENT
-------------------------------------
Result of alignment is displayed on standard output. Result will contain of a sequence of words, each followed by it's start and end time in the utterance as detected by Long Audio aligner.

Eg. Sphinx(1.01,1.37)

  Word detected  : Sphinx
  Start Time	   : 1.01 sec
  End Time	     : 1.37 sec
