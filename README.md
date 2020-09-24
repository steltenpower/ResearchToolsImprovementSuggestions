# ResearchToolsImprovementSuggestions
I see little and big confusion and other room for improvement while supporting Endnote, Qualtrics, atlas.ti and others which made me write down some remarks below

But first, to understand me a bit better:

I'd like manuals mostly diagrams in this order:
- Core concepts
- where does data live, in what (preferably open) formats
- Typical flow of cooperation
- "UI/commands are 'self-explaining', details show up where you need them. There's no manual for them, just a reference, that gladly is hardly used"

Endnote basic:
==============
- Find in Cite-While-You-Write needs to show nr of references searched through, fuzzy search and the ability to change which groups shared with you are also searched through
- Easier to install on more browsers and more word processors
- when DOI is available, use that to retrieve metadata.
- Show what Wayback machine has for webcontent and offer to submit snapshot of current state
- Allow multiple file upload for "Import references"
- For both import and export use what the filetype implies
- Rename the concept of Groups. Is it a Folder? Is it a filter (based on tags)? Also to make "find duplicates" easier to grasp
- rename&reorder Collect: "Search Online | New Reference | Import References" into "Search | Import | Create (capture/manually)"
- Some day we'll escape simulating the paper era and have [citation styles as a reading option[(https://github.com/steltenpower/CitationStyleOnReading), instead of a 'print' option.
 

Qualtrics:
==========
- Explain how multi-select works when a respondent hits the first (many people don't know how to work the control and shift buttons for this). Especially confusing when there are more options than fit the window or scrollbox as you can then inadvertantly unselect options you can't see.
- Say why you don't accept a list of e-mail addresses (there are empty or otherwise invalid entries in there. Leading and trailing spaces are hard to see, but wrong.) Preferably show which e-mail addresses are the problem.
- Think about how to change something quickly on loads of questions simultaneously.
- Think about how to use all screen space on a 40"+ 4K screen
- Design questions and resulting data-format at the same time (one, can follow the other, and vice versa)
- Keep respondents from reply-ing by e-mail with complaints/questions, but keep it in context.
- Getting people to respond a 2nd time to a survey is even harder. Therefore do your utmost to prevent people from mailing out surveys with problems, especially to many at the same time.
- Who decided on the default style for your account? Qualtrics? The buyer? Mine makes different kinds of questions look the same. And wastes screen space because of too much emptyness

atlas.ti:
=========
- Do some renaming. Even official trainers shorten Quotations to Quotes, which then sound too similar to codes; "part"?
Coding is programming to many; "tag"?
Document is 3 syllables; "source"? But "sources" is 2; "files"? "content"?
- Some redesign exercises to improve the program:
  - Maximize space for content, minimize space for menus
  - It's a multi-user program
  - It's web-based
  - Linked Data as data format (see also https://github.com/steltenpower/mapping-between-REFI-QDA-and-LODcloud )
  - multi-touch
  - Version control is done through Git(hub), not from within atlas.ti (That is how more and more people work, also thanks to open science)
  - What are primary constructs, what are convenience things? Make that obvious somehow.
  - Focus on clear and powerful core concepts (it's just a few things). The (even with tiny characters) thick 'quick' and massive 'full' manuals and the giant menus are confusing/scaring people

SURF research drive:
====================
= built on ownCloud
===================

-Three ways to serve files please:
1. download (you are asked/forced to save the file somewhere)
2. open in a server-side (generated) environment (e.g. a PDF reader)
3. (as 1, but with HTTP-header "content-disposition" ignored) let the web browser handle the file directly. Useful for example for HTML files using JavaScript to load CSV files to visualize. Of course this could be done elsewhere, but then you have to repeat defining the same access regime.

-Extra's for displaying files in a folder (which for implementation could maybe tap into file type descriptions on wikidata):
1. Green checkmark if the file validates: consistent file content matches with file type extension (especially those listed as [DANS' preferred formats](https://dans.knaw.nl/en/about/services/easy/information-about-depositing-data/before-depositing/file-formats?set_language=en). To help prevent problems with interoperability, a term you might know from FAIR data, which should have started with an I. I-FAR maybe?
2. In contextMenu of a file (preferably also when viewed through webDAV), related installed applications are shown, followed by those easily available from SURF.nl or Github (open source is part of open science after all). Also link to the technical specification of the file type. This should advance data-centric thinking, especially as it's not uncommon to hear "I don't know. I work with (app) X. what's this vendor lock-in you mention?"
3. Also for data-centric thinking: File icons based on file type (not primary associated application). For example not a Chrome or Firefox icon for HTML or SVG files.
