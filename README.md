# YData: Humanities Data Mining

This repository contains materials for YData: Humanities Data Mining (S&DS 176 / S&DS 576), taught in the Spring of 2022 at Yale University. For more information on the course, please consult the preliminary  [**syllabus**](https://github.com/YaleDHLab/humanities-data-mining/blob/master/YDATA-HumanitiesDataMiningSpring2022.pdf) or the course materials below (please note that some materials require a Yale NetID for access).

You can also view the syllabus from the first year the class was taught, [Spring 2021](https://github.com/YaleDHLab/humanities-data-mining/blob/master/Spring-2021.md).

### Week One: Introduction to Data Mining

In our first week, of class we will discuss some of the ways researchers from the humanities and beyond have used data mining, and we will take our first steps with the Python programming language.

[**Tuesday Slides**](https://docs.google.com/presentation/d/1kIM6ts5PnacRHk0YdGWvMY4ecgSnrTD32cdMUjjU2Hk/edit?usp=sharing)<br/>
[**Thursday Lab Notebook**](https://colab.research.google.com/drive/1ynzXjh0hKbdJIj0LtQuPFn-SaCWY3rPi?usp=sharing)<br/>
**Readings**<br/>
* Michael Witmore, “[Text: A Massively Addressable Object](https://dhdebates.gc.cuny.edu/read/untitled-88c11800-9446-469b-a3be-3fdb36bfbd1e/section/402e7e9a-359b-4b11-8386-a1b48e40425a)”
* Ted Underwood, “[Seven ways humanists are using computers to understand text](https://tedunderwood.com/2015/06/04/seven-ways-humanists-are-using-computers-to-understand-text/)”

### Week Two: Collecting Data from APIs

In our second week, of class we will take a deeper dive into data--what it is, how it's created, and how we can find and use it. In particular, we'll explore Application Programming Interfaces (APIs)--little machines that give us data to analyze!

[**Tuesday Slides**](https://docs.google.com/presentation/d/1nqA0TBXOnypuXMFtO4x6huMVGFabx41VT9Bd62fmT2s/edit?usp=sharing)<br/>
**Readings**<br/>
* Christof Schöch, &ldquo;<a class="inline_disabled" href="http://journalofdigitalhumanities.org/2-3/big-smart-clean-messy-data-in-the-humanities/" target="_blank" rel="noopener noreferrer">Big? Smart?&nbsp; Clean? Messy? Data in the Humanities</a>&rdquo;
* Johanna Drucker, &ldquo;<a class="inline_disabled" href="https://www.cambridge.org/core/services/aop-cambridge-core/content/view/757C1225CFDCF629FC2895C76DD747B0/S0030812900116098a.pdf/why-distant-reading-isnt.pdf" target="_blank" rel="noopener noreferrer">Why Distant Reading Isn&rsquo;t</a>&rdquo;<span style="font-size: 8pt;"> (VPN or on-campus network needed)</span>


### Week Three: Data Visualization

[**Tuesday Slides**](https://docs.google.com/presentation/d/17pd5CL-bfPI5da3igAc8fDlLh2KDbdynATUK-G1OQtg/edit?usp=sharing)<br/>
[**Thursday Lab Tutorial**](https://github.com/YaleDHLab/humanities-data-mining/blob/master/workshop-materials/tableau-workshop/README.md)<br/>
**Readings**<br/>
* Catherine D’Ignazio and Lauren Klein, “<a href="http://www.kanarinka.com/wp-content/uploads/2015/07/IEEE_Feminist_Data_Visualization.pdf">Feminist Data Visualization”</a>

In our third week, we will consider strategies and best practices for visualizing data that take into account what kind of data we have, who we have in mind as our audience, what story we're aiming to tell, and where we think the visualization will circulate. For Thursday's lab, please download [Tableau Public](https://public.tableau.com/en-us/s/).

<i>No problem set assigned this week -- Work on Project Review 1: Text Mining. You can find the prompt in Canvas under "Assignments."</i>

### Week Four: Text Analysis: Named Entity Recognition

In our fourth week, we will begin turning our attention to text analysis in more detail. In particular, we will experiment with an approach called named entity recognition, which can help us extract entities (names, locations, organizations) from text.
**Readings**<br/>
<ul>
    <li>Richard Jean So, &ldquo;<a class="inline_disabled" href="https://www.cambridge.org/core/journals/pmla/article/all-models-are-wrong/0AFE2CEA7F036769916EC819BFCD8E6E#" target="_blank" rel="noopener">All Models are Wrong</a>&rdquo;</li>
    <li>Jean Baptiste-Michel et al. &ldquo;<a class="inline_disabled" href="https://www.science.org/doi/10.1126/science.1199644" target="_blank" rel="noopener">Quantitative Analysis of Culture Using Millions of Digitized Books</a>&rdquo;</li>
</ul>

### Week Five: Clustering and Classification

In our fifth week, we will explore supervised methods for classifying and clustering data using Python. We will consider when such approaches could be helpful, as well as what the limitations are and what kind of data we need to have.
**Readings**<br/>
<ul>
    <li>Patrick Juola, &ldquo;<a class="inline_disabled" href="https://www.scientificamerican.com/article/how-a-computer-program-helped-show-jk-rowling-write-a-cuckoos-calling/" target="_blank" rel="noopener">How a Computer Program Helped Show J.K. Rowling write <em>A Cuckoo&rsquo;s Calling</em></a>&rdquo; [sic]</li>
    <li>Franco Moretti, "<a class="inline_disabled" href="https://muse.jhu.edu/article/22852" target="_blank" rel="noopener">The Slaughterhouse of Literature</a>" [on-campus network or <a class="inline_disabled" href="https://ask.library.yale.edu/faq/174875" target="_blank" rel="noopener">VPN</a> required]</li>
</ul>

### Week Six: Review and Topic Modeling 

In our sixth week, we will review several of the programming topics we have covered so far in the semester, and we'll explore a few new topics that will prove useful as we continue our data science work in the coming weeks. We will learn about topic modeling by looking at case studies and experimenting with model parameters. The particular approach we'll be using is called non-negative matrix factorization (NMF), which like the classifier we trained in week five, starts with a Term-Document Matrix.

**Readings**<br/>
<ul>
    <li>Underwood, Ted. "<a class="inline_disabled" href="https://tedunderwood.com/2012/04/07/topic-modeling-made-just-simple-enough/" target="_blank" rel="noopener">Topic Modeling Made Just Simple Enough</a>"</li>
    <li>Blevins, Cameron. "<a class="inline_disabled" href="https://www.cameronblevins.org/posts/topic-modeling-martha-ballards-diary/" target="_blank" rel="noopener">Topic Modeling Martha Ballard's Diary</a>"</li>
</ul>

### Week Seven: Text & Image Analysis: Neural Networks

In our seventh week, we will begin our transition from text mining to image mining techniques by way of neural networks. On Thursday, we will focus on word embeddings, a technique for identifying words that appear in similar contexts.

**[Tuesday Slides](https://docs.google.com/presentation/d/1wj-5EjLEMRg7boOlrXB9TSOwMmjw0WNryyz_phBN4VI/edit?usp=sharing)**

**Readings**<br/>
<ul>
    <li>Gideon Lewis-Kraus, &ldquo;<a class="inline_disabled" href="https://www.nytimes.com/2016/12/14/magazine/the-great-ai-awakening.html" target="_blank" rel="noopener">The Great A.I. Awakening</a>&rdquo;</li>
    <li>Jonathan Fitzgerald, &ldquo;<a class="inline_disabled" href="https://cssh.northeastern.edu/nulab/word-embedding-models-new-topic-models/" target="_blank" rel="noopener">Word Embeddings are the New Topic Models</a>&rdquo;</li>
    <li>Optional: Ryan Heuser, &ldquo;<a href="https://ryanheuser.org/word-vectors/)">Word Vectors in the Eighteenth Century</a>&rdquo;<li>
    <li>Optional: Ben Schmidt, &ldquo;<a href="http://bookworm.benschmidt.org/posts/2015-10-25-Word-Embeddings.html">Vector Space Models for the Digital Humanities</a>&rdquo;</li>
</ul>

**[Thursday Notebook](https://colab.research.google.com/drive/1tGrSqgTyE1heKZuWxifPi-lHvjfeBYdr?usp=sharing)**

**[Thursday Problem Set](https://colab.research.google.com/drive/15qeboVR-U51Hk_F27Aua-MpwVmEQjuhf?usp=sharing)**

### Week Eight: Computer Vision: Color & Art 

In our eighth week, we will start looking more closely at image mining, with an overview of projects, techniques, and data considerations. For hands-on practice, we will experiment with color extraction.

**[Tuesday Slides](https://docs.google.com/presentation/d/1JS28si7_P9FSWN8ybp5XogCPR6sZfINVu2lIVq2KWN8/edit?usp=sharing)**

**Tuesday Readings**:

* [The True Colors of America’s Political Spectrum Are Gray and Green](https://www.nytimes.com/interactive/2020/09/02/upshot/america-political-spectrum.html)

**Thursday Notebooks and links**:

* [Color Analysis in Python](https://colab.research.google.com/drive/1MH-qZfIG30qRFUxWP7IZw4AQDFGtgy3w?usp=sharing)
* [Visualizing Colors in RGB Space](https://colab.research.google.com/drive/1Z7N_GD3PIDa2Ta2Ae7l2VmvON9FtXVma?usp=sharing)
* [Visualizing clustering in HSV space](http://dh.library.yale.edu/projects/vogue/colorcluster.html)

### Week Nine: Spring Recess

### Week 10: Visual Similarity

In our tenth week, we will be discussing techniques for measuring and identifying image similarity. In particular, we will focus on Convolutional Neural Networks as our approach.

**Tuesday Readings:**

* [The visual digital turn: Using neural networks to study historical images](https://academic.oup.com/dsh/article/35/1/194/5296356)

**[Tuesday Slides](https://docs.google.com/presentation/d/1BF7USpA4xqZ2zoLSkywJ7CvaF2nakILTvm8uITBeLeI/edit?usp=sharing)**

**Tuesday In-Class Links:**

* [Lyrics Text Comparison](https://colab.research.google.com/drive/1ImjzOLnxxfM0qcjD8K1rOugkJziGUzZz?usp=sharing)
* [Image Similarity Ordering](https://cderose.github.io/image-similarity/)
* [Neural Neighbors](https://dhlab.yale.edu/neural-neighbors/) (Meserve-Kunhardt Collection)

**Thursday Notebooks:**

* [Image Similarity](https://colab.research.google.com/drive/1nI-7QOaWgepRDBcATIe6EylsYvibZg9j?usp=sharing)
* [Building PixPlot Visualizations with your own images](https://colab.research.google.com/drive/1eQg6yAXUDM_XdS5E1PmZ5J_BhJBclEhi?usp=sharing)

### Week 11: Image, Video and Music Analaysis

In our eleventh week, we will look at methods for video (or moving image) analysis and consider when, why, and how we might go about it. As a capstone to our image analysis module, we will use the [Distant Viewing Toolkit](https://github.com/distant-viewing/dvt). We'll also explore classifing sound files according to musical genre with guest lecturer Nicole Cosme (Yale Music Department).

**[Tuesday Slides](https://docs.google.com/presentation/d/1B1w3gLd_27xebM43urhVlI8-XaKOwqtBvYBH-05lREY/edit?usp=sharing)**<br>
**Tuesday Notebook**
* [Distant Viewing Toolkit (DVT) Demo](https://colab.research.google.com/drive/1gRUI8LRtCUpCfglTHNsPwx4e_NoUBSSU?usp=sharing)<br>

**Tuesday Readings**
* [Distant viewing: analyzing large visual corpora](https://academic.oup.com/dsh/article/34/Supplement_1/i3/5694340)
* Optional: [Unraveling the JPEG](https://parametric.press/issue-01/unraveling-the-jpeg/)

### Week 12: Open Lab 1, Finding and Preparing Data

In our twelfth week, we will begin our open lab sessions, which are designed to pull together the material from the course while giving you time to work on your final projects. For our first open lab, we will discuss pathways for finding and preparing data.

### Week 13: Open Labs 2 & 3, Analyzing and Visualizing Data

In our thirtienth week, we will continue bringing the course material together by discussing how to identify an appropriate method based on your research question and available data. We will also review strategies for visualizing and sharing results. 

### Week 14: Presentations

In our fourteenth week, we will conclude with class presentations to showcase everyone's work. Thank you for an incredible semester!


## Acknowledgements
The course materials are published under a CC BY 3.0 US license. This course, Humanities Data Mining, was created in 2021 by Dr. Catherine DeRose and Dr. Douglas Duhaime.
