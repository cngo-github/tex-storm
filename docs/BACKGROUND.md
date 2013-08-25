BACKGROUND
==========
When I was trying to set up a near real-time information extraction system at work that could scale horizontally, I looked at both UIMA and Storm.  However, there was no open source natural language processing (NLP) implementation for Storm.  Given the constraint on resources, I recommended that that team pursue the more developed UIMA NLP system instead, despite Storm being the more appropriate architecture for the our needs.  Since that time, I still have been unable to find an open source NLP project built around Storm.  Tex Storm is meant to provide a starting point for anyone looking to develop an NLP system based around Storm.