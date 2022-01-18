The framework package contains the base components required for running the SimpleNLG package. The components can be split into four different categories. The first category contains only the NLGModule abstract class. This module is used to define processors that will run in the SimpleNLG package. Some example basic processors are included with the application and they all extend this class. Note that modules and processors are interchangeable in this documentation. They both refer to a class that extends the NLGModule base class.

The second category of components are formed from the elements. Elements in SimpleNLG form the document structure, phrases, clauses, canned text and the words themselves. There are numerous Element classes all of which extend from the top-level abstract class NLGElement. Generic modules can be written to run with the generic NLGElement class. The other element classes are:

CoordinatedPhraseElement - used for coordinating phrases together through the use of conjunctions such as and and but.
DocumentElement - defines document structure of a text to the level of document, section, paragraph and sentences.
InflectedWordElement - represents a word that needs to be inflected.
ListElement - a single element entity representing a list of NLGElements and should not be confused with List<NLGElement>
PhraseElement - defines the phrases of the text such as: clauses, noun phrases and verb phrases.
StringElement - a canned text representation that is not meant to be changed by any of the processors.
WordElement - a representation of a base word as read from the lexicon definition.
The third set of components are the enumerated types representing the different categories for the elements. All the enumerations implement the ElementCategory interface. This allows for generic modules to access a generic category type. The other enumerations are:

DocumentCategory - defines which part of the document structure the DocumentElement represents. For example, sentence and paragraph.
LexicalCategory - represents the types of grammatical categories for the individual words. For example, noun, verb and adjective.
PhraseCategory - details the type of phrase a PhraseElement represents. For example, noun phrase, clause, prepositional phrase.
The final category covers the two factories. The factories should be used to construct other elements. They are: DocumentFactory, which constructs document elements pertaining to the text structure; and PhraseFactory, which constructs various types of phrases.