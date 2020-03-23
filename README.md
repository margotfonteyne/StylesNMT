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
## Citing
The data set is free to use for research purposes. Please cite the following paper if you use it in your research:<br>
* Fonteyne, M., Macken, L., and Tezcan, A. (forthcoming). Literary Machine Translation under the Magnifying Glass: Assessing the Quality of an NMT-Translated Detective Novel on Document Level. In *Proceedings of the Twelfth International Conference on Language Resources and Evaluation (LREC 2020)*, Marseille, France, May 13-15, 2020: European Language Resources Association (ELRA).
## References
* Tezcan, A., Hoste, V., and Macken, L. (2017). Scate taxonomy and corpus of machine translation errors. In Gloria Corpas Pastor et al., editors, *Trends in E-tools and resources for translators and interpreters, volume 45 of Approaches to Translation Studies*, pages 219–244. Brill — Rodopi.
