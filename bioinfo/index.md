| Overview | Bioinformatics | Scientific Software Development | HPC | Teaching

## Bioinformatics Team

The bioinformatics team assists MPI-CBG scientists with a wide range of bioinformatics data analysis tasks.  Services range from small scale single gene or protein characterization up to global studies involving deep sequencing technologies.


### NGS applications

NGS data analysis workflows are designed to run in an HPC environment and include automated report generation using R/markdown, linking to underlying source data and/or QC reports. We are currently also developing a RNA-seq analysis workflow single cell data.

<table style="text-align:center;">
  <tr>
    <th><i>Step</i></th>
    <th><i>Tool</i></th>
    <th><i>Deliverable</i></th>
  </tr>
  
  <tr><td colspan="3"></td></tr>
  
  <tr>
    <td colspan="3" style="background:#c53233;color:white;text-shadow: 2px 2px 5px black;"><b>Steps common to all workflows</b></td>
  </tr>
    <tr>
    <td>Reads QC</td>
    <td>FastQC</td>
    <td>Html Report</td>
  </tr>
  <tr>
    <td>Functional Analysis</td>
    <td>ClusterProfiler (R), PathView (R), KEGGRest (R), Enrichr, WCGNA</td>
    <td>HTML report, Tab-delimited files, charts</td>
  </tr>
  
  <tr><td colspan="3"></td></tr>
  
  <tr>
  <td colspan="3" style="background:#2b67ac;color:white;text-shadow: 2px 2px 5px black;"><b>Transcriptome Profiling*</b></td>
  </tr>
    <tr>
    <td>Alignment</td>
    <td>STAR</td>
    <td>QC HTML report & Bam files</td>
  </tr>
  <tr>
    <td>Quantification</td>
    <td>HTSeq or FeatureCounts (STAR)</td>
    <td>Count tables & HTML report</td>
  </tr>
  <tr>
    <td>Differential Expression</td>
    <td>DESeq2, DEXSeq, CuffDiff</td>
    <td>HTML Report, Tab-delimited files</td>
  </tr>
  
  <tr><td colspan="3"></td></tr>
  
  <tr>
  <td colspan="3" style="background:#2b67ac;color:white;text-shadow: 2px 2px 5px black;"><b><i>De novo</i> Transcriptome Assembly</b></td>
  </tr>
    <tr>
    <td><i>De novo</i> assembly</td>
    <td>Trinity</td>
    <td>Fasta file</td>
  </tr>
  <tr>
    <td>Annotation</td>
    <td>Blastx, InterProScan, HMMer, TreeFAM, BUSCO</td>
    <td>HTML report and tab delimited files</td>
  </tr>
  <tr>
    <td>Quantification</td>
    <td>Trinity (RSEM)</td>
    <td>HTML report and tab delimited files</td>
  </tr>
  <tr>
    <td>Differential Expression</td>
    <td>EdgeR, DESeq</td>
    <td>HTML report and tab delimited files</td>
  </tr>
  
  <tr><td colspan="3"></td></tr>
  
  <tr>
  <td colspan="3" style="background:#2b67ac;color:white;text-shadow: 2px 2px 5px black;"><b>ChIP-Seq</b></td>
  </tr>
    <tr>
    <td>Alignment & QC</td>
    <td>Bowtie2, PicardTools, deepTools</td>
    <td>Bam files</td>
  </tr>
  <tr>
    <td>Peak Calling</td>
    <td>Macs2, Sicer</td>
    <td>Bed files, HTML Report, Tab-delimited files</td>
  </tr>
  <tr>
    <td>Annotation</td>
    <td>ChIPPeakAnno (R)</td>
    <td>HTML report and tab delimited files</td>
  </tr>
  <tr>
    <td>Motif Analysis</td>
    <td>Meme</td>
    <td>HTML report and tab delimited files</td>
  </tr>
  <tr>
    <td>Differential Binding</td>
    <td>DiffBind</td>
    <td>HTML report, Tab-delimited files, charts</td>
  </tr>
  
    <tr><td colspan="3"></td></tr>
  
  <tr>
  <td colspan="3" style="background:#2b67ac;color:white;text-shadow: 2px 2px 5px black;"><b>Variant Calling</b></td>
  </tr>
    <tr>
    <td>Alignment & QC</td>
    <td>BWA, Bowtie2</td>
    <td>Bam files</td>
  </tr>
  <tr>
    <td>Variant Calling & QC</td>
    <td>bcfTools, samtools, pilon</td>
    <td>Bed files, HTML Report, Tab-delimited files</td>
  </tr>
</table>

### Useful links
[Bioinformatics gitlab repo](https://git.mpi-cbg.de/bioinfo)

[Scientific Computing gitlab repo](https://git.mpi-cbg.de/scicomp)

### Publications
<div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Marta Florio, Michael Heide, Anneline Pinson, Holger Brandl, Mareike Albert, Sylke Winkler, Pauline Wimberger, Wieland B. Huttner, Michael Hiller<br/>
<span class="pubtitle">Evolution and cell-type specificity of human-specific genes preferentially expressed in progenitors of fetal neocortex.</span><br/>
<span class="journal_name">Elife</span>, 7 Art. No. e32332 (2018)<br/>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/29561261" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.7554/eLife.32332" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract7090" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex7090" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract7090"><div class="well">Understanding the molecular basis that underlies the expansion of the neocortex during primate, and notably human, evolution requires the identification of genes that are particularly active in the neural stem and progenitor cells of the developing neocortex. Here, we have used existing transcriptome datasets to carry out a comprehensive screen for protein-coding genes preferentially expressed in progenitors of fetal human neocortex. We show that fifteen human-specific genes exhibit such expression, and many of them evolved distinct neural progenitor cell-type expression profiles and levels compared to their ancestral paralogs. Functional studies on one such gene,NOTCH2NL, demonstrate its ability to promote basal progenitor proliferation in mice. An additional 35 human genes with progenitor-enriched expression are shown to have orthologs only in primates. Our study provides a resource of genes that are promising candidates to exert specific, and novel, roles in neocortical development during primate, and notably human, evolution.</div></div><div class="collapse" id="bibtex7090"><div class="well">@article{Florio7090,<br>   author={Marta Florio, Michael Heide, Anneline Pinson, Holger Brandl, Mareike Albert, Sylke Winkler, Pauline Wimberger, Wieland B. Huttner, Michael Hiller},<br>   title={Evolution and cell-type specificity of human-specific genes preferentially expressed in progenitors of fetal neocortex.},<br>   journal={eLife},<br>   volume={7},<br>   pages={null--null},<br>   year=2018<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Markus Grohme, Siegfried Schloissnig, Andrei Rozanski, Martin Pippel, George Robert Young, Sylke Winkler, Holger Brandl, Ian Henry, Andreas Dahl, Sean Powell, Michael Hiller, Eugene Myers, Jochen Rink<br/>
<span class="pubtitle">The genome of Schmidtea mediterranea and the evolution of core cellular mechanisms.</span><br/>
<span class="journal_name">Nature</span>, 554(7690) 56-61 (2018)<br/>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/29364871" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.1038/nature25473" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract7065" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex7065" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract7065"><div class="well">The planarian Schmidtea mediterranea is an important model for stem cell research and regeneration, but adequate genome resources for this species have been lacking. Here we report a highly contiguous genome assembly of S. mediterranea, using long-read sequencing and a de novo assembler (MARVEL) enhanced for low-complexity reads. The S. mediterranea genome is highly polymorphic and repetitive, and harbours a novel class of giant retroelements. Furthermore, the genome assembly lacks a number of highly conserved genes, including critical components of the mitotic spindle assembly checkpoint, but planarians maintain checkpoint function. Our genome assembly provides a key model system resource that will be useful for studying regeneration and the evolutionary plasticity of core cell biological mechanisms.</div></div><div class="collapse" id="bibtex7065"><div class="well">@article{Grohme7065,<br>   author={Markus Grohme, Siegfried Schloissnig, Andrei Rozanski, Martin Pippel, George Robert Young, Sylke Winkler, Holger Brandl, Ian Henry, Andreas Dahl, Sean Powell, Michael Hiller, Eugene Myers, Jochen Rink},<br>   title={The genome of Schmidtea mediterranea and the evolution of core cellular mechanisms.},<br>   journal={Nature},<br>   volume={554},<br>   issue ={7690},<br>   pages={56--61},<br>   year=2018<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Ioannis Mitroulis, Klara Ruppova, Baomei Wang, Lan-Sun Chen, Michal Grzybek, Tatyana Grinenko, Anne Eugster, Maria Troullinaki, Alessandra Palladini, Ioannis Kourtzelis, Antonios Chatzigeorgiou, Andreas Schlitzer, Marc Beyer, Leo A B Joosten, Berend Isermann, Mathias Lesche, Andreas Petzold, Kai Simons, Ian Henry, Andreas Dahl, Joachim L Schultze, Ben Wielockx, Nicola Zamboni, Peter Mirtschink, Ünal Coskun, George Hajishengallis, Mihai G Netea, Trian  Chavakis<br/>
<span class="pubtitle">Modulation of Myelopoiesis Progenitors Is an Integral Component of Trained Immunity.</span><br/>
<span class="journal_name">Cell</span>, 172(1-2) 147-161 (2018)<br/>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/29328910" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.1016/j.cell.2017.11.034" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract7033" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex7033" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract7033"><div class="well">Trained innate immunity fosters a sustained favorable response of myeloid cells to a secondary challenge, despite their short lifespan in circulation. We thus hypothesized that trained immunity acts via modulation of hematopoietic stem and progenitor cells (HSPCs). Administration of β-glucan (prototypical trained-immunity-inducing agonist) to mice induced expansion of progenitors of the myeloid lineage, which was associated with elevated signaling by innate immune mediators, such as IL-1β and granulocyte-macrophage colony-stimulating factor (GM-CSF), and with adaptations in glucose metabolism and cholesterol biosynthesis. The trained-immunity-related increase in myelopoiesis resulted in a beneficial response to secondary LPS challenge and protection from chemotherapy-induced myelosuppression in mice. Therefore, modulation of myeloid progenitors in the bone marrow is an integral component of trained immunity, which to date, was considered to involve functional changes of mature myeloid cells in the periphery.</div></div><div class="collapse" id="bibtex7033"><div class="well">@article{Mitroulis7033,<br>   author={Ioannis Mitroulis, Klara Ruppova, Baomei Wang, Lan-Sun Chen, Michal Grzybek, Tatyana Grinenko, Anne Eugster, Maria Troullinaki, Alessandra Palladini, Ioannis Kourtzelis, Antonios Chatzigeorgiou, Andreas Schlitzer, Marc Beyer, Leo A B Joosten, Berend Isermann, Mathias Lesche, Andreas Petzold, Kai Simons, Ian Henry, Andreas Dahl, Joachim L Schultze, Ben Wielockx, Nicola Zamboni, Peter Mirtschink, Ünal Coskun, George Hajishengallis, Mihai G Netea, Trian  Chavakis},<br>   title={Modulation of Myelopoiesis Progenitors Is an Integral Component of Trained Immunity.},<br>   journal={Cell},<br>   volume={172},<br>   issue ={1-2},<br>   pages={147--161},<br>   year=2018<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Ivana Viktorinová, Ian Henry, Pavel Tomancak<br/>
<span class="pubtitle">Epithelial rotation is preceded by planar symmetry breaking of actomyosin and protects epithelial tissue from cell deformations.</span><br/>
<span class="journal_name">PLoS Genet</span>, 13(11) Art. No. 1007107 (2017)<br/>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/29176774" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.1371/journal.pgen.1007107" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract6980" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex6980" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract6980"><div class="well">Symmetry breaking is involved in many developmental processes that form bodies and organs. One of them is the epithelial rotation of developing tubular and acinar organs. However, how epithelial cells move, how they break symmetry to define their common direction, and what function rotational epithelial motions have remains elusive. Here, we identify a dynamic actomyosin network that breaks symmetry at the basal surface of the Drosophila follicle epithelium of acinar-like primitive organs, called egg chambers, and may represent a candidate force-generation mechanism that underlies the unidirectional motion of this epithelial tissue. We provide evidence that the atypical cadherin Fat2, a key planar cell polarity regulator in Drosophila oogenesis, directs and orchestrates transmission of the intracellular actomyosin asymmetry cue onto a tissue plane in order to break planar actomyosin symmetry, facilitate epithelial rotation in the opposite direction, and direct the elongation of follicle cells. In contrast, loss of this rotational motion results in anisotropic non-muscle Myosin II pulses that are disorganized in plane and causes cell deformations in the epithelial tissue of Drosophila eggs. Our work demonstrates that atypical cadherins play an important role in the control of symmetry breaking of cellular mechanics in order to facilitate tissue motion and model epithelial tissue. We propose that their functions may be evolutionarily conserved in tubular/acinar vertebrate organs.</div></div><div class="collapse" id="bibtex6980"><div class="well">@article{Viktorinová6980,<br>   author={Ivana Viktorinová, Ian Henry, Pavel Tomancak},<br>   title={Epithelial rotation is preceded by planar symmetry breaking of actomyosin and protects epithelial tissue from cell deformations.},<br>   journal={PLoS genetics},<br>   volume={13},<br>   issue ={11},<br>   pages={null--null},<br>   year=2017<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Barbara Tavares, Raquel Jacinto, Pedro Sampaio, Sara Pestana, Andreia Pinto, Andreia Vaz, Mónica Roxo-Rosa, Rui Gardner, Telma Lopes, Britta Schilling, Ian Henry, Leonor Saúde, Susana Lopes<br/>
<span class="pubtitle">Notch/Her12 signalling modulates, motile/immotile cilia ratio downstream of Foxj1a in zebrafish left-right organizer.</span><br/>
<span class="journal_name">Elife</span>, 6 Art. No. e25165 (2017)<br/>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/28875937" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.7554/eLife.25165" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract6931" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex6931" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract6931"><div class="well">Foxj1a is necessary and sufficient to specify motile cilia. Using transcriptional studies and slow-scan two-photon live imaging capable of identifying the number of motile and immotile cilia, we now established that the final number of motile cilia depends on Notch signalling (NS). We found that despite all left-right organizer (LRO) cells express foxj1a and the ciliary axonemes of these cells have dynein arms, some cilia remain immotile. We identified that this decision is taken early in development in the Kupffer's Vesicle (KV) precursors the readout being her12 transcription. We demonstrate that overexpression of either her12 or Notch intracellular domain (NICD) increases the number of immotile cilia at the expense of motile cilia, and leads to an accumulation of immotile cilia at the anterior half of the KV. This disrupts the normal fluid flow intensity and pattern, with consequent impact on dand5 expression pattern and left-right (L-R) axis establishment.</div></div><div class="collapse" id="bibtex6931"><div class="well">@article{Tavares6931,<br>   author={Barbara Tavares, Raquel Jacinto, Pedro Sampaio, Sara Pestana, Andreia Pinto, Andreia Vaz, Mónica Roxo-Rosa, Rui Gardner, Telma Lopes, Britta Schilling, Ian Henry, Leonor Saúde, Susana Lopes},<br>   title={Notch/Her12 signalling modulates, motile/immotile cilia ratio downstream of Foxj1a in zebrafish left-right organizer.},<br>   journal={eLife},<br>   volume={6},<br>   pages={null--null},<br>   year=2017<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Mareike Albert, Nereo Kalebic, Marta Florio, Naharajan Lakshmanaperumal, Christiane Haffner, Holger Brandl, Ian Henry, Wieland B. Huttner<br/>
<span class="pubtitle">Epigenome profiling and editing of neocortical progenitor cells during development.</span><br/>
<span class="journal_name">EMBO J</span>, 36(17) 2642-2658 (2017)<br/>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/28765163" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.15252/embj.201796764" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract6924" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex6924" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract6924"><div class="well">The generation of neocortical neurons from neural progenitor cells (NPCs) is primarily controlled by transcription factors binding to DNA in the context of chromatin. To understand the complex layer of regulation that orchestrates different NPC types from the same DNA sequence, epigenome maps with cell type resolution are required. Here, we present genomewide histone methylation maps for distinct neural cell populations in the developing mouse neocortex. Using different chromatin features, we identify potential novel regulators of cortical NPCs. Moreover, we identify extensive H3K27me3 changes between NPC subtypes coinciding with major developmental and cell biological transitions. Interestingly, we detect dynamic H3K27me3 changes on promoters of several crucial transcription factors, including the basal progenitor regulator Eomes We use catalytically inactive Cas9 fused with the histone methyltransferase Ezh2 to edit H3K27me3 at the Eomes locus in vivo, which results in reduced Tbr2 expression and lower basal progenitor abundance, underscoring the relevance of dynamic H3K27me3 changes during neocortex development. Taken together, we provide a rich resource of neocortical histone methylation data and outline an approach to investigate its contribution to the regulation of selected genes during neocortical development.</div></div><div class="collapse" id="bibtex6924"><div class="well">@article{Albert6924,<br>   author={Mareike Albert, Nereo Kalebic, Marta Florio, Naharajan Lakshmanaperumal, Christiane Haffner, Holger Brandl, Ian Henry, Wieland B. Huttner},<br>   title={Epigenome profiling and editing of neocortical progenitor cells during development.},<br>   journal={The EMBO journal},<br>   volume={36},<br>   issue ={17},<br>   pages={2642--2658},<br>   year=2017<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Peter Steinbach, Matthias Werner<br/>
<span class="pubtitle">gearshifft – The FFT Benchmark Suite for Heterogeneous Platforms</span><br/>
<i>
In: High performance computing ; 32nd international conference, ISC High Performance 2017, Frankfurt, Germany, June 18-22, 2017 : proceedings </i>
(2017)(Eds.) Julian Kunkel (Lecture Notes in Computer Science ; 10266), Cham, Springer International Publishing (2017), 199-216
<br/>
<a href="http://dx.doi.org/10.1007/978-3-319-58667-0_11" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex6923" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="bibtex6923"><div class="well">@proceedings{Steinbach6923,<br>   title        = {gearshifft – The FFT Benchmark Suite for Heterogeneous Platforms},<br>   year         = 2017,<br>   editor       = {Peter Steinbach, Matthias Werner},<br>   volume       = {High performance computing ; 32nd international conference, ISC High Performance 2017, Frankfurt, Germany, June 18-22, 2017 : proceedings },<br>   series       = {(Lecture Notes in Computer Science ; 10266)},<br>   publisher    = {Springer International Publishing}<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Helge Knoop, Tobias Gronemeier, Christoph Knigge, Peter Steinbach<br/>
<span class="pubtitle">Porting the MPI Parallelized LES Model PALM to Multi-GPU Systems – An Experience Report</span><br/>
<i>
In: High performance computing : ISC High Performance 2016 international workshops ExaComm, E-MuCoCoS, HPC-IODC, IXPUG, IWOPH, P^3MA, VHPC, WOPSSS, Frankfurt, Germany, June 19-23, 2016 : revised selected papers</i>
(2016) Lecture Notes in Computer Science ; 9945, Cham, Springer International Publishing (2016), 508-523
<br/>
<a href="http://dx.doi.org/10.1007/978-3-319-46079-6_35" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex6736" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="bibtex6736"><div class="well">@proceedings{Knoop6736,<br>   title        = {Porting the MPI Parallelized LES Model PALM to Multi-GPU Systems – An Experience Report},<br>   year         = 2016,<br>   editor       = {Helge Knoop, Tobias Gronemeier, Christoph Knigge, Peter Steinbach},<br>   volume       = {High performance computing : ISC High Performance 2016 international workshops ExaComm, E-MuCoCoS, HPC-IODC, IXPUG, IWOPH, P^3MA, VHPC, WOPSSS, Frankfurt, Germany, June 19-23, 2016 : revised selected papers},<br>   series       = {Lecture Notes in Computer Science ; 9945},<br>   publisher    = {Springer International Publishing}<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Kristin Stützer, Robert Haase, Fabian Lohaus, Steffen Barczyk, Florian Exner, Steffen Löck, Jan Rühaak, Bianca Lassen-Schmidt, Dörte Corr, Constance Richter<br/>
<span class="pubtitle">Evaluation of a deformable registration algorithm for subsequent lung computed tomography imaging during radiochemotherapy.</span><br/>
<span class="journal_name">Med Phys</span>, 43(9) 5028-5028 (2016)<br/>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/27587033" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.1118/1.4960366" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract6685" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex6685" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract6685"><div class="well">Rating both a lung segmentation algorithm and a deformable image registration (DIR) algorithm for subsequent lung computed tomography (CT) images by different evaluation techniques. Furthermore, investigating the relative performance and the correlation of the different evaluation techniques to address their potential value in a clinical setting.</div></div><div class="collapse" id="bibtex6685"><div class="well">@article{Stützer6685,<br>   author={Kristin Stützer, Robert Haase, Fabian Lohaus, Steffen Barczyk, Florian Exner, Steffen Löck, Jan Rühaak, Bianca Lassen-Schmidt, Dörte Corr, Constance Richter},<br>   title={Evaluation of a deformable registration algorithm for subsequent lung computed tomography imaging during radiochemotherapy.},<br>   journal={Medical physics},<br>   volume={43},<br>   issue ={9},<br>   pages={5028--5028},<br>   year=2016<br>}</div></div></p>
                        </large>
                    </div>
                </div>
            
                <div class="row topbuffer">
                    <div class="col-md-10">
                        <large>
                            <p class="publication">Raphael Etournay, Matthias Merkel, Marko Popović, Holger Brandl, Natalie Dye, Benoit Aigouy, Guillaume Salbreux, Suzanne Eaton, Frank Jülicher<br/>
<span class="pubtitle">TissueMiner: a multiscale analysis toolkit to quantify how cellular processes create tissue dynamics.</span><br/>
<span class="journal_name">Elife</span>, 5 Art. No. e14334 (2016)<br/>
<a href="/Etournay_2016_6556.pdf"><img align="top" src="/images/iconset/application_pdf.png"/></a>&nbsp;&nbsp;<a href="http://www.ncbi.nlm.nih.gov/pubmed/27228153" class="btn btn-default btn-xs" role="button">PubMed</a>&nbsp;<a href="http://dx.doi.org/10.7554/eLife.14334" class="btn btn-default btn-xs" role="button">Source</a>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#abstract6556" data-toggle="collapse"">Abstract</button>&nbsp;<button type="button" class="btn btn-default btn-xs" href="#bibtex6556" data-toggle="collapse"">BibTex</button>&nbsp;<div class="collapse" id="abstract6556"><div class="well">Segmentation and tracking of cells in long-term time-lapse experiments has emerged as a powerful method to understand how tissue shape changes emerge from the complex choreography of constituent cells. However, methods to store and interrogate the large datasets produced by these experiments are not widely available. Furthermore, recently developed methods for relating tissue shape changes to cell dynamics have not yet been widely applied by biologists because of their technical complexity. We therefore developed a database format that stores cellular connectivity and geometry information of deforming epithelial tissues, and computational tools to interrogate it and perform multi-scale analysis of morphogenesis. We provide tutorials for this computational framework, called TissueMiner, and demonstrate its capabilities by comparing cell and tissue dynamics in vein and inter-vein subregions of the Drosophila pupal wing. These analyses reveal an unexpected role for convergent extension in shaping wing veins.</div></div><div class="collapse" id="bibtex6556"><div class="well">@article{Etournay6556,<br>   author={Raphael Etournay, Matthias Merkel, Marko Popović, Holger Brandl, Natalie Dye, Benoit Aigouy, Guillaume Salbreux, Suzanne Eaton, Frank Jülicher},<br>   title={TissueMiner: a multiscale analysis toolkit to quantify how cellular processes create tissue dynamics.},<br>   journal={eLife},<br>   volume={5},<br>   pages={null--null},<br>   year=2016<br>}</div></div></p>
                        </large>
                    </div>
                </div>
