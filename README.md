# Various documents related to Tesseract OCR


## [The Fourth Annual Test of OCR Accuracy](AT-1995.pdf)

Publication Year: 1995

## [An Overview of the Tesseract OCR Engine](tesseracticdar2007.pdf)

Publication Year: 2007

The Tesseract OCR engine, as was the HP Research Prototype in the UNLV Fourth Annual Test of OCR Accuracy[1], is described in a comprehensive overview. Emphasis is placed on aspects that are novel or at least unusual in an OCR engine, including in particular the line finding, features/classification methods, and the adaptive classifier.

## [Hybrid Page Layout Analysis via Tab-Stop Detection](PageLayoutAnalysisICDAR2.pdf)

Published at [2009 10 th International Conference on Document Analysis and Recognition](https://dblp1.uni-trier.de/db/conf/icdar/icdar2007.html).

([source](https://ai.google/research/pubs/pub35094))

A new hybrid page layout analysis algorithm is proposed, which uses bottom-up methods to form an initial data-type hypothesis and locate the tab-stops that were used when the page was formatted. The detected tab-stops are used to deduce the column layout of the page. The column layout is then applied in a top-down manner to impose structure and reading-order on the detected regions. The complete C++ source code implementation is available as part of the Tesseract open source OCR engine athttps://github.com/tesseract-ocr/tesseract.

## [Combined Orientation and Script Detection using the Tesseract OCR Engine](Combined_Orientation_and_Script_Detection_using_the_Tesseract_OCR_Engine.pdf)

([source](https://ai.google/research/pubs/pub35506))

Publication Year: 2009

This paper proposes a simple but effective algorithm to estimate the script and dominant page orientation of the text contained in an image. A candidate set of shape classes for each script is generated using synthetically rendered text and used to train a fast shape classifier. At run time, the classifier is applied independently to connected components in the image for each possible orientation of the component, and the accumulated confidence scores are used to determine the best estimate of page orientation and script. Results demonstrate the effectiveness of the approach on a dataset of 1846 documents containing a diverse set of images in 14 scripts and any of four possible page orientations.

## [Adapting the Tesseract Open Source OCR Engine for Multilingual OCR](MOCRadaptingtesseract2.pdf)

([source](https://ai.google/research/pubs/pub35248))

Publication Year: 2009

We describe efforts to adapt the Tesseract open source OCR engine for multiple scripts and languages. Effort has been concentrated on enabling generic multi-lingual operation such that negligible customization is required for a new language beyond providing a corpus of text. Although change was required to various modules, including physical layout analysis, and linguistic post-processing, no change was required to the character classifier beyond changing a few limits. The Tesseract classifier has adapted easily to Simplified Chinese. Test results on English, a mixture of European languages, and Russian, taken from a random sample of books, show a reasonably consistent word error rate between 3.72% and 5.78%, and Simplified Chinese has a character error rate of only 3.77%.

©ACM, 2009. This is the authors’ version of the work. It is posted here by permission of ACM for your personal use. Not for redistribution. The definitive version was published in Proceedings of the International Workshop on Multilingual OCR 2009, Barcelona, Spain July 25, 2009.


## [Table detection in heterogeneous documents](Table_detection_in_heterogeneous_documents.pdf)

([source](https://ai.google/research/pubs/pub35652))

Publication Year: 2010

Detecting tables in document images is important since not only do tables contain important information, but also most of the layout analysis methods fail in the presence of tables in the document image. Existing approaches for table detection mainly focus on detecting tables in single columns of text and do not work reliably on documents with varying layouts. This paper presents a practical algorithm for table detection that works with a high accuracy on documents with varying layouts (company reports, newspaper articles, magazine pages, ...). An open source implementation of the algorithm is provided as part of the Tesseract OCR engine. Evaluation of the algorithm on document images from publicly available UNLV dataset shows competitive performance in comparison to the table detection module of a commercial OCR system.

Comparison to other implementation:
* [Learning to Detect Tables in Scanned Document Images
using Line Information](https://hal.archives-ouvertes.fr/hal-00934902/file/ICDAR_table_detection.pdf) at 2017 14th IAPR International Conference on Document Analysis and Recognition 
* [Table Detection using Deep Learning](https://www.researchgate.net/publication/320243569_Table_Detection_Using_Deep_Learning)


## [Limits on the Application of Frequency-based Language Models to OCR](Limits_on_the_Application_of_Frequency-based_Language_Models_to_OCR.pdf)

([source](https://ai.google/research/pubs/pub36984))

Publication Year: 2011

Although large language models are used in speech recognition and machine translation applications, OCR systems are “far behind” in their use of language models. The reason for this is not the laggardness of the OCR community, but the fact that, at high accuracies, a frequency-based language model can do more damage than good, unless carefully applied. This paper presents an analysis of this discrepancy with the help of the Google Books n-gram Corpus, and concludes that noisy-channel models that closely model the underlying classifier and segmentation errors are required.


## [Improving Book OCR by Adaptive Language and Image Models](Improving_Book_OCR_by_Adaptive_Language_and_Image_Models.pdf)

([source](https://ai.google/research/pubs/pub37481))

Publication Year: 2012

In order to cope with the vast diversity of book content and typefaces, it is important for OCR systems to leverage the strong consistency within a book but adapt to variations across books. In this work, we describe a system that combines two parallel correction paths using document-specific image and language models. Each model adapts to shapes and vocabularies within a book to identify inconsistencies as correction hypotheses, but relies on the other for effective cross-validation. Using the open source Tesseract engine as baseline, results on a large dataset of scanned books demonstrate that word error rates can be reduced by 25% using this approach.

## Tesseract Blends Old and New OCR Technology: Tutorial2 at [DAS2016 – Document Analysis Systems](https://www.primaresearch.org/das2016/tutorials)

  * [Tutorial Contents](das_tutorial2016/0TutorialContents.pdf)
  * [Motivation and History of the Tesseract OCR Engine](das_tutorial2016/1Intro-history.pdf)
  * [Architecture and Data Structures](das_tutorial2016/2ArchitectureAndDataStructures.pdf)
  * [Features and Character Classifier](das_tutorial2016/3CharacterClassifiers.pdf)
  * [Character Segmentation, Language Models and Beam Search](das_tutorial2016/4CharSegmentation.pdf)
  * [Page Layout Analysis](das_tutorial2016/5LayoutAnalysis.pdf)
  * [Modernization Efforts](das_tutorial2016/6ModernizationEfforts.pdf)
  * [Building a Multilingual OCR Engine](das_tutorial2016/7Building%20a%20Multi-Lingual%20OCR%20Engine.pdf)

