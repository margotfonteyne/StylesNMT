# StylesNMT
This data repository contains an English-Dutch machine translation (MT) of the detective novel "The Mysterious Affair at Styles" by Agatha Christie. The translation was generated in May 2019 by Google's neural MT system. The complete novel (5,276 sentence pairs) has been manually annotated with translation errors using an adapted version of the SCATE MT error taxonomy (Tezcan et al. 2017). The data set was annotated in [WebAnno](https://webanno.github.io/webanno/), a web-based annotation tool.
![The adapted SCATE MT error taxonomy](/images/taxonomy.png)
## Data set details
The novel was split into multiple parts (13 in total) to ease the annotation process. In total, two annotators worked independently on the data set. The first annotator annotated the complete novel, the second only the first chapter of the novel. Their annotations can be found in the files ending with "anno1" and "anno2" respectively.
## File structure
### WebAnno_Project.zip
ZIP file containing the project as exported from WebAnno, including all settings (layers, tagsets, guidelines, etc.) and annotations. It can be easily imported in WebAnno (see the section on [importing projects](https://webanno.github.io/webanno/releases/3.6.4/docs/user-guide.html#_import) in the tool's [user guide](https://webanno.github.io/webanno/releases/3.6.4/docs/user-guide.html)).
### WebAnno_Annotations-xmi.zip
ZIP file containing the exported annotations in [UIMA XMI](https://uima.apache.org/d/uimaj-current/references.html#ugr.ref.xmi) file format. In this format, the annotations can be processed in Python with the help of the [DKPro cassis](https://github.com/dkpro/dkpro-cassis) library.
### WebAnno_Annotations-tsv.zip
ZIP file containing the exported annotations in [WebAnno TSV3](https://webanno.github.io/webanno/releases/3.6.4/docs/user-guide.html#sect_webannotsv) file format.
### AnnotationGuidelines.pdf
PDF containing the guidelines used to annotate the novel.
## Citing
The data set is free to use for research purposes. Please cite the following paper if you use it in your research:<br>
* Fonteyne, M., Tezcan, A., & Macken, L. (2020). Literary machine translation under the magnifying glass : assessing the quality of an NMT-translated detective novel on document level. In N. Calzolari, F. Béchet, P. Blache, K. Choukri, C. Cieri, T. Declerck, … S. Piperidis (Eds.), *12th International Conference on Language Resources and Evaluation Conference (LREC 2020), Proceedings* (pp. 3783–3791). Paris, France: European Language Resources Association (ELRA).
## References
* Tezcan, A., Hoste, V., & Macken, L. (2017). SCATE taxonomy and corpus of machine translation errors. In G. C. Pastor & I. Durán-Muñoz (Eds.), *Trends in E-tools and resources for translators and interpreters* (Vol. 45, pp. 219–244). Brill | Rodopi.
