WCE-SLT-LIG
===========


Corpus for evaluation of WCE in Spoken Language Translation

======

This corpus contains 6693 speech utterances (DEV: 2643 speech utterances; TST: 4050 speech utterances) for which a quintuplet containing: ASR output (src-asr), verbatim transcript (src-ref), text translation output (tgt-mt), speech translation output (tgt-slt) and post-edition of translation (tgt-pe), is made available.


If you are using this corpus please cite the following paper (pdf given on this root directory):

@InProceedings{besacier14,
  Title                    = {Word Confidence Estimation for Speech Translation},
  Author                   = {Laurent Besacier and Benjamin Lecouteux and Ngoc Quang Luong and Kaing Hour and Marwa Hadjsalah},
  Booktitle                = {Proceedings of The International Workshop on Spoken Language Translation (IWSLT)},
  Year                     = {2014},

  Address                  = {Lake Tahoe, USA},
  Month                    = {December},

  Date-added               = {2014-10-01 07:42:11 +0000},
  Date-modified            = {2014-10-01 07:44:40 +0000}
}


The paper above describes the V1 of this corpus available in CORPUS-V1.old directory (2683 utterances only).
The other folders described below correspond to the new and full version of this corpus (6693 utterances).

========================================================================
The folder WAV_TRANSCRIPTION contains the 6693 speech signals recorded and transcriptions (DEV: 2643 speech signals recorded; TST: 4050 speech signals recorded)

The folder TXT contains the following files:
Source Language (French)
./SRC/
     10881     268285    1761184 SRC/src-ref-all.fr              => 10881 sentences in French (all)
          
       881      20315     132195 SRC/src-ref-dev.fr              => 881 sentences in French (REF Output for dev part)
      2643      65964     397461 SRC/ref-asr-dev-3times.fr.pre   => 881*3 sentences in French (ASR Reference for dev part)
      
      1350      33784     225462 SRC/src-ref-tst.fr              => 1350 sentences in French (REF Output for tst part)
      4050     109212     681789 SRC/ref-asr-tst-3times.fr.pre   => 1350*3 sentences in French (ASR Reference for tst part)
      
./SRC/ASR1/
      2643      66435     395274 SRC/ASR1/scr-asr-dev-3times.fr  => 881*3 sentences in French (ASR1 Hypothesis for dev part)
      4050     108333     671792 SRC/ASR1/scr-asr-tst-3times.fr  => 1350*3 sentences in French (ASR1 Hypothesis for tst part)

./SRC/ASR2/   
      2643      66837     396883 SRC/ASR2/scr-asr-dev-3times.fr  => 881*3 sentences in French (ASR2 Hypothesis for dev part)
      4050     108600     674572 SRC/ASR2/scr-asr-tst-3times.fr  => 1350*3 sentences in French (ASR2 Hypothesis for tst part)
          
     
Target Language (English)
./TGT/
     10881     251410    1522348 TGT/tgt-pe-all.en               => 10881 post-edition of MT sentences in English (all)     
       881      19606     117857 TGT/tgt-pe-dev.en               => 881 post-edition of MT sentences in English (dev part)       
      2643      58818     353571 TGT/tgt-pe-dev-3times.en        => 881*3 post-edition of MT sentences in English (dev part)      
      1350      31396     193176 TGT/tgt-pe-tst.en               => 1350 post-edition of MT sentences in English (tst part)      
      4050      94029     578415 TGT/tgt-pe-tst-3times.en        => 1350*3 post-edition of MT sentences in English (tst part)
      
     10881     238190    1473247 TGT/tgt-ref-all.en              => 10881 manually translated sentences in English (all)
       881      18490     112884 TGT/tgt-ref-dev.en              => 881 manually translated sentences in English (dev part)      
      1350      28886     183741 TGT/tgt-ref-tst.en              => 1350 manually translated sentences in English (tst part)      

     10881     281868    1542560 TGT/tgt-mt-all.en               => 10881 automatically translated sentences in English (all)
       881      22340     120183 TGT/tgt-mt-dev.en               => 881 automatically translated sentences in English (dev part)       
      1350      35213     197574 TGT/tgt-mt-tst.en               => 1350 automatically translated sentences in English (tst part)
      
./TGT/ASR1/
      2643      61787     352660 TGT/ASR1/tgt-slt-dev-3times.en  => 881*3 SLT (ASR+MT) sentences in English (ASR+MT hypothesis for dev part)
      4050      97977     581357 TGT/ASR1/tgt-slt-tst-3times.en  => 1350*3 SLT (ASR+MT) sentences in English (ASR+MT hypothesis for tst part)

./TGT/ASR2/
      2643      62213     354786 TGT/ASR2/tgt-slt-dev-3times.en  => 881*3 SLT (ASR+MT) sentences in English (ASR+MT hypothesis for dev part)
      4050      97804     581655 TGT/ASR2/tgt-slt-tst-3times.en  => 1350*3 SLT (ASR+MT) sentences in English (ASR+MT hypothesis for tst part)
      
      
Labels by calculating WER or TERp-A
./Labels/
     15897     187714    1441827 Labels/Labels-ASR1-dev.pra      => obtained from WER(scr-asr-dev-3times.fr of ASR1, ref-asr-dev-3times.fr.pre)
     24363     297838    2402596 Labels/Labels-ASR1-tst.pra      => obtained from WER(scr-asr-tst-3times.fr of ASR1, ref-asr-tst-3times.fr.pre)
     15897     184286    1432164 Labels/Labels-ASR2-dev.pra      => obtained from WER(scr-asr-dev-3times.fr of ASR2, ref-asr-dev-3times.fr.pre)
     24363     292032    2388547 Labels/Labels-ASR2-tst.pra      => obtained from WER(scr-asr-tst-3times.fr of ASR2, ref-asr-tst-3times.fr.pre)
     
     15182     193887    1115346 Labels/Labels-MT-dev.pra        => obtained from TERp-A(tgt-mt-dev.en, tgt-pe-dev.en)
     23092     301782    1780907 Labels/Labels-MT-tst.pra        => obtained from TERp-A(tgt-mt-tst.en, tgt-pe-tst.en)
     
     45556     556446    3286938 Labels/Labels-SLT-ASR1-dev.pra  => obtained from TERp-A(tgt-slt-dev-3times.en of ASR1, tgt-pe-dev-3times.en)
     69582     870117    5270874 Labels/Labels-SLT-ASR1-tst.pra  => obtained from TERp-A(tgt-slt-tst-3times.en of ASR1, tgt-pe-tst-3times.en)
     45472     558097    3290231 Labels/Labels-SLT-ASR2-dev.pra  => obtained from TERp-A(tgt-slt-dev-3times.en of ASR2, tgt-pe-dev-3times.en)
     69439     867842    5259856 Labels/Labels-SLT-ASR2-tst.pra  => obtained from TERp-A(tgt-slt-tst-3times.en of ASR2, tgt-pe-tst-3times.en) 

