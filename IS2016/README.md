# SLT Corpus for INTERSPEECH 2016 paper

This repository contains all the corpora used in the paper submitted to the INTERSPEECH 2016.
The paper can be found in the directory "paper".

## A new ASR metric: WER-S

This corpus was use to select the best ASR output according to the following metrics: the WER and its extension WER-S.
The last metric is a simple new extension of the WER metric in order to penalize differently substitution errors according to their context using word embeddings.
For instance, the proposed metric should catch near matches (mainly morphological variants) and penalize less this kind oferror which has a more limited impact on translation performance. 
Our experiments show that the correlation of the new proposed metric with SLT performance is better than the one of WER. <br />
Oracle experiments are also conducted and show the ability of our metric to find better hypotheses (to be translated) in the ASR N-best. 
Finally, a preliminary experiment where ASR tuning is based on our new metric shows encouraging results. 
For reproductible experiments, the code allowing to call our modified WER and the corpora used are made available to the research community.

## WER-S code

here you can find a description of the new metrics used in these experiments:
https://github.com/cservan/tercpp-embeddings

## Organisation

<a href=".">.</a><br>
├── <a href="./paper/">paper</a><br>
├── <a href="./ASR_outputs/">ASR_outputs</a><br>
│   ├── <a href="./ASR_outputs/best_scale_WER/">best_scale_WER</a><br>
│   ├── <a href="./ASR_outputs/best_scale_WER-S/">best_scale_WER-S</a><br>
│   │   └── <a href="./ASR_outputs/best_scale_WER-S/NBest/">NBest</a><br>
│   ├── <a href="./ASR_outputs/references/">references</a><br>
│   └── <a href="./ASR_outputs/scale_from_01_to_20/">scale_from_01_to_20</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_01/">scale_01</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_02/">scale_02</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_03/">scale_03</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_04/">scale_04</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_05/">scale_05</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_06/">scale_06</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_07/">scale_07</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_08/">scale_08</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_09/">scale_09</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_10/">scale_10</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_11/">scale_11</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_12/">scale_12</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_13/">scale_13</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_14/">scale_14</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_15/">scale_15</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_16/">scale_16</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_17/">scale_17</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_18/">scale_18</a><br>
│   &nbsp;&nbsp;&nbsp; ├── <a href="./ASR_outputs/scale_from_01_to_20/scale_19/">scale_19</a><br>
│   &nbsp;&nbsp;&nbsp; └── <a href="./ASR_outputs/scale_from_01_to_20/scale_20/">scale_20</a><br>
└── <a href="./SLT_outputs/">SLT_outputs</a><br>
&nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/1-Best_ASR/">1-Best_ASR</a><br>
&nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/oracle_ASR_WER/">oracle_ASR_WER</a><br>
&nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/oracle_ASR_WER-E/">oracle_ASR_WER-E</a><br>
&nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/oracle_ASR_WER-S/">oracle_ASR_WER-S</a><br>
&nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/references_ASR/">references_ASR</a><br>
&nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/references_SLT/">references_SLT</a><br>
&nbsp;&nbsp;&nbsp; └── <a href="./SLT_outputs/scale_from_01_to_20/">scale_from_01_to_20</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_01/">scale_01</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_02/">scale_02</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_03/">scale_03</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_04/">scale_04</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_05/">scale_05</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_06/">scale_06</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_07/">scale_07</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_08/">scale_08</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_09/">scale_09</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_10/">scale_10</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_11/">scale_11</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_12/">scale_12</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_13/">scale_13</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_14/">scale_14</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_15/">scale_15</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_16/">scale_16</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_17/">scale_17</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_18/">scale_18</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ├── <a href="./SLT_outputs/scale_from_01_to_20/scale_19/">scale_19</a><br>
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; └── <a href="./SLT_outputs/scale_from_01_to_20/scale_20/">scale_20</a><br>
<br><br>
