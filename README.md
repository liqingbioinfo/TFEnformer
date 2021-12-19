# TFEnformer
Genome-wide association studies (GWASs) have identified a substantial amount of genetic variants associated with diseases, but identifying the causal SNP(s) or gene(s) remains a major challenge. In this project, we develop TFEnformer, which transfers distal regulatory knowledge learned by Enformer and integrates the tissue-specific non-transcribed Transcription Factors [TFs] to prioritize the causal SNP(s) or gene(s) in specific tissues and diseases. 

By utilizing transfer learning, this TFEnformer has two advantages:
1. Since the majority of its weights are transferred from the well-trained Enformer model, TFEnformer automatically takes account of 84% (<100 kb) genome distal regulatory elements such as enhancers, repressors, and insulators. 
2. TFEnformer is trained on tissue-specific non-transcribed TFs, which grants this model the power to recognize tissue-specific SNPs. 

##Setup
###Requirements:
- dm-sonnet (2.0.0)
- kipoiseq (0.5.2)
- numpy (1.19.5)
- pandas (1.2.3)
- tensoflow (2.4.1)
- tensorflow-hub (0.11.0)
See requirements.txt.

```
python3.8 -m venv TFEnformer_venv
source TFEnformer_venv/bin/activate
pip install -r requirements.txt
```
