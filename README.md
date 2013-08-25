Tex-Storm
=========

An implementation of a NLP system built around the Storm project based on what I've learned working with GATE, Stanford NLP, and UIMA and it's associated projects.

BACKGROUND
==========
When I was trying to set up a near real-time information extraction system at work that could scale horizontally, I looked at both UIMA and Storm.  However, there was no open source natural language processing (NLP) implementation for Storm.  Given the constraint on resources, I recommended that that team pursue the more developed UIMA NLP system instead, despite Storm being the more appropriate architecture for the our needs.  Since that time, I still have been unable to find an open source NLP project built around Storm.  Tex Storm is meant to provide a starting point for anyone looking to develop an NLP system based around Storm.

GOALS
=====
The goal of Tex Storm is to develop a natural language processing (NLP) system built around the Storm project.  This will allow Tex Storm to be horizontally scalable and capable of real-time processing.  It should be easy to customize the various NLP components do whatever is desired.  Tex Storm, in addition to NLP processing of text documents, should also be capable of handling non-text data sources as well as transforming text documents to meet the needs of the user.

The development of Tex Storm will be heavily informed by the General Architecture for Text Engineering (GATE), Stanford NLP, and Apache Unstructured Information Management Architecture and its derivative projects.  Due to the scale of the project, development will be, initially, focused on English, well formed, low-noise documents, and broken into 5 phases:

- Development of a rules-based NLP system.
- Generalization of the project to allow it to process non-text documents, given the correct processors.
- Development of an ability to modify the text document during processing.
- Development of a models-based NLP system.
- Extend the NLP system for additional capabilities (ontologies, sentiment analysis, etc...)

Current Work
============
Please see the proposal for phase 1: /docs/PROPOSAL_PHASE01.md

The first task is to implement a rules-based system.  This will be based upon A Nearly New Information Extraction (ANNIE) system.  ANNIE is from the General Architecture for Text Engineering (GATE), which can be found at:

	http://gate.ac.uk/

Initial work will be aimed at replicating the basic ANNIE in terms of capability as well as building the system to allow it to be easily modified and expand them.  In order to accomplish this, the following things will need to be implemented:

- Construct the base system to handle documents and feed them through the Storm topology.
- Construct the needed components to analyze the documents or processing resources in GATE lingo.
	- Segmenter
	- Tokenizer
	- Part-of-speech Tagger
	- Named Entity Recognizer
