GOALS
=====
The goal of Tex Storm is to develop a natural language processing (NLP) system built around the Storm project.  This will allow Tex Storm to be horizontally scalable and capable of real-time processing.  It should be easy to customize the various NLP components do whatever is desired.  Tex Storm, in addition to NLP processing of text documents, should also be capable of handling non-text data sources as well as transforming text documents to meet the needs of the user.

The development of Tex Storm will be heavily informed by the General Architecture for Text Engineering (GATE), Stanford NLP, and Apache Unstructured Information Management Architecture and its derivative projects.  Due to the scale of the project, development will be, initially, focused on English, well formed, low-noise documents, and broken into 5 phases:

- Development of a rules-based NLP system.
- Generalization of the project to allow it to process non-text documents, given the correct processors.
- Development of an ability to modify the text document during processing.
- Development of a models-based NLP system.
- Extend the NLP system for additional capabilities (ontologies, sentiment analysis, etc...)
