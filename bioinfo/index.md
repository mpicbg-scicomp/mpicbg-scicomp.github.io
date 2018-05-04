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
Marta Florio, Michael Heide, Anneline Pinson, Holger Brandl, Mareike Albert, Sylke Winkler, Pauline Wimberger, Wieland B. Huttner, Michael Hiller
Evolution and cell-type specificity of human-specific genes preferentially expressed in progenitors of fetal neocortex.
Elife, 7 Art. No. e32332 (2018)

Markus Grohme, Siegfried Schloissnig, Andrei Rozanski, Martin Pippel, George Robert Young, Sylke Winkler, Holger Brandl, Ian Henry, Andreas Dahl, Sean Powell, Michael Hiller, Eugene Myers, Jochen Rink
The genome of Schmidtea mediterranea and the evolution of core cellular mechanisms.
Nature, 554(7690) 56-61 (2018)

Ioannis Mitroulis, Klara Ruppova, Baomei Wang, Lan-Sun Chen, Michal Grzybek, Tatyana Grinenko, Anne Eugster, Maria Troullinaki, Alessandra Palladini, Ioannis Kourtzelis, Antonios Chatzigeorgiou, Andreas Schlitzer, Marc Beyer, Leo A B Joosten, Berend Isermann, Mathias Lesche, Andreas Petzold, Kai Simons, Ian Henry, Andreas Dahl, Joachim L Schultze, Ben Wielockx, Nicola Zamboni, Peter Mirtschink, Ünal Coskun, George Hajishengallis, Mihai G Netea, Trian Chavakis
Modulation of Myelopoiesis Progenitors Is an Integral Component of Trained Immunity.
Cell, 172(1-2) 147-161 (2018)

Ivana Viktorinová, Ian Henry, Pavel Tomancak
Epithelial rotation is preceded by planar symmetry breaking of actomyosin and protects epithelial tissue from cell deformations.
PLoS Genet, 13(11) Art. No. 1007107 (2017)

Barbara Tavares, Raquel Jacinto, Pedro Sampaio, Sara Pestana, Andreia Pinto, Andreia Vaz, Mónica Roxo-Rosa, Rui Gardner, Telma Lopes, Britta Schilling, Ian Henry, Leonor Saúde, Susana Lopes
Notch/Her12 signalling modulates, motile/immotile cilia ratio downstream of Foxj1a in zebrafish left-right organizer.
Elife, 6 Art. No. e25165 (2017)

Mareike Albert, Nereo Kalebic, Marta Florio, Naharajan Lakshmanaperumal, Christiane Haffner, Holger Brandl, Ian Henry, Wieland B. Huttner
Epigenome profiling and editing of neocortical progenitor cells during development.
EMBO J, 36(17) 2642-2658 (2017)

Peter Steinbach, Matthias Werner
gearshifft – The FFT Benchmark Suite for Heterogeneous Platforms
In: High performance computing ; 32nd international conference, ISC High Performance 2017, Frankfurt, Germany, June 18-22, 2017 : proceedings (2017)(Eds.) Julian Kunkel (Lecture Notes in Computer Science ; 10266), Cham, Springer International Publishing (2017), 199-216

Helge Knoop, Tobias Gronemeier, Christoph Knigge, Peter Steinbach
Porting the MPI Parallelized LES Model PALM to Multi-GPU Systems – An Experience Report
In: High performance computing : ISC High Performance 2016 international workshops ExaComm, E-MuCoCoS, HPC-IODC, IXPUG, IWOPH, P^3MA, VHPC, WOPSSS, Frankfurt, Germany, June 19-23, 2016 : revised selected papers (2016) Lecture Notes in Computer Science ; 9945, Cham, Springer International Publishing (2016), 508-523

Kristin Stützer, Robert Haase, Fabian Lohaus, Steffen Barczyk, Florian Exner, Steffen Löck, Jan Rühaak, Bianca Lassen-Schmidt, Dörte Corr, Constance Richter
Evaluation of a deformable registration algorithm for subsequent lung computed tomography imaging during radiochemotherapy.
Med Phys, 43(9) 5028-5028 (2016)

Raphael Etournay, Matthias Merkel, Marko Popović, Holger Brandl, Natalie Dye, Benoit Aigouy, Guillaume Salbreux, Suzanne Eaton, Frank Jülicher
TissueMiner: a multiscale analysis toolkit to quantify how cellular processes create tissue dynamics.
Elife, 5 Art. No. e14334 (2016)

Falk Tillner, Prasad Thute, Steffen Löck, Antje Dietrich, Andriy Fursov, Robert Haase, Mathias Lukas, Bernd Rimarzig, Manfred Sobiella, Mechthild Krause, Michael Baumann, Rebecca Bütof, Wolfgang Enghardt
Precise image-guided irradiation of small animals: a flexible non-profit platform.
Phys Med Biol, 61(8) 3084-3108 (2016)

Christopher Schmied, Peter Steinbach, Tobias Pietzsch, Stephan Preibisch, Pavel Tomancak
An automated workflow for parallel processing of large multiview SPIM recordings.
Bioinformatics, 32(7) 1112-1114 (2016)

Michaela Müller-McNicoll, Valentina Botti, Antonio Domingues, Holger Brandl, Oliver D Schwich, Michaela Steiner, Tomaz Curk, Ina Poser, Kathi Zarnack, Karla M. Neugebauer
SR proteins are NXF1 adaptors that link alternative RNA processing to mRNA export.
Genes Dev, 30(5) 553-566 (2016)

L Carine Stapel, Benoit Lombardot, Coleman Broaddus, Dagmar Kainmueller, Florian Jug, Eugene W Myers, Nadine Vastenhouw
Automated detection and quantification of single RNAs at cellular resolution in zebrafish embryos.
Development, 143(3) 540-546 (2016)

Holger Brandl, HongKee Moon, Miquel Vila-Farré, Shang-Yun Liu, Ian Henry, Jochen Rink
PlanMine - a mineable resource of planarian biology and biodiversity.
Nucleic Acids Res, 44 Art. No. D764–D773 (2016)

Mykola Mylenko, Sebastian Boland, Sider Penkov, Julio Sampaio, Benoit Lombardot, Daniela Vorkel, Jean-Marc Verbavatz, Teymuras V. Kurzchalia
NAD+ Is a Food Component That Promotes Exit from Dauer Diapause in Caenorhabditis elegans.
PLoS ONE, 11(12) Art. No. e0167208 (2016)

Anja Zeigerer, Roman L Bogorad, Kirti Sharma, Jerome Gilleron, Sarah Seifert, Susanne Sales, Nikolaus Berndt, Sascha Bulik, Giovanni Marsico, Rochelle C J D'Souza, Naharajan Lakshmanaperumal, Kesavan Meganathan, Karthick Natarajan, Agapios Sachinidis, Andreas Dahl, Hermann-Georg Holzhütter, Andrej Shevchenko, Matthias Mann, Victor Koteliansky, Marino Zerial
Regulation of Liver Metabolism by the Endosomal GTPase Rab5.
Cell Rep, 11(6) 884-892 (2015)

Stefan Kluth, Maria Grazia Pia, Thomas Schoerner-Sadenius, Peter Steinbach
How do particle physicists learn the programming concepts they need?
In: 21ST INTERNATIONAL CONFERENCE ON COMPUTING IN HIGH ENERGY AND NUCLEAR PHYSICS (CHEP2015), PARTS 1-9 (2015) Ch. 62048 (Journal of Physics Conference Series ; 664,6), Bristol, UK, Institute of Physics Publishing (IOP) (2015)

Marta Florio, Mareike Albert, Elena Taverna, Takashi Namba, Holger Brandl, Eric Lewitus, Christiane Haffner, Alex Sykes, Fong Kuan Wong, Jula Peters, E. Guhr, Sylvia Klemroth, Kay Prüfer, Janet Kelso, Ronald Naumann, Ina Nüsslein, Andreas Dahl, Robert Lachmann, Svante Pääbo, Wieland B. Huttner
Human-specific gene ARHGAP11B promotes basal progenitor amplification and neocortex expansion.
Science, 347(6229) 1465-1470 (2015)

Raphael Etournay, Marko Popović, Matthias Merkel, Amitabha Nandi, Corinna Blasse, Benoit Aigouy, Holger Brandl, Gene Myers, Guillaume Salbreux, Frank Jülicher, Suzanne Eaton
Interplay of cell dynamics and epithelial tension during morphogenesis of the Drosophila pupal wing.
Elife, 4 Art. No. e07090 (2015)

Hanh Thi-Kim Vu, Jochen Rink, Sean A McKinney, Melainia McClain, Naharajan Lakshmanaperumal, Richard Alexander, Alejandro Sánchez Alvarado
Stem cells and fluid flow drive cyst formation in an invertebrate excretory organ.
Elife, 4 Art. No. e07405 (2015)

Tatyana Grinenko, Kathrin Arndt, Melanie Portz, Nicole Mende, Marko Günther, Kadriye Nehir Cosgun, Dimitra Alexopoulou, Naharajan Lakshmanaperumal, Ian Henry, Andreas Dahl, Claudia Waskow
Clonal expansion capacity defines two consecutive developmental stages of long-term hematopoietic stem cells.
J Exp Med, 211(2) 209-215 (2014)

Shang-Yun Liu, Claudia Selck, Benjamin Friedrich, Richard Lutz, Miquel Vila-Farré, Andreas Dahl, Holger Brandl, Naharajan Lakshmanaperumal, Ian Henry, Jochen Rink
Reactivating head regrowth in a regeneration-deficient planarian species.
Nature, 500(7460) 81-84 (2013)

Simone Fietz, Robert Lachmann, Holger Brandl, Martin Kircher, Nikolay Samusik, Roland Schröder, Naharajan Lakshmanaperumal, Ian Henry, Johannes Vogt, Axel Riehn, Wolfgang Distler, Robert Nitsch, Wolfgang Enard, Svante Pääbo, Wieland B. Huttner
Transcriptomes of germinal zones of human and mouse fetal neocortex suggest a role of extracellular matrix in progenitor self-renewal.
Proc Natl Acad Sci U.S.A., 109(29) 11836-11841 (2012)
