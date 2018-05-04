| Overview | Bioinformatics | Scientific Software Development | HPC | Teaching

## Bioinformatics Team

The bioinformatics team assists MPI-CBG scientists with a wide range of bioinformatics data analysis tasks.  Services range from small scale single gene or protein characterization up to global studies involving deep sequencing technologies.


### NGS applications
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
