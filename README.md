## Papers on deep learning/machine learning for proteins

### Basic idea

This repository collects Deep learning/Machine learning papers for protein research (especially antigen-antibody). The idea is derived from [Kevin Yang](https://github.com/yangkky/Machine-learning-for-proteins)

### Categories

[Reviews](#reviews)   
[Predicting structure](#predicting-structure)   
[Classification](#classification-and-annotation)    
[Predicting interactions](#predicting-interactions)   
[Generative models](#generative-models)   
[Representation learning with self-supervised learning](#representation-learning-with-self-supervised-learning)    

### Reviews

**Deep Learning in Protein Structural Modeling and Design**     
[Gao, Wenhao, et al. Patterns (2020): 100142.](https://doi.org/10.1016/j.patter.2020.100142)

### Predicting structure
[Transformer]
**Highly accurate protein structure prediction with AlphaFold**   
[Jumper, John, et al. Nature 596.7873 (2021): 583-589.](https://doi.org/10.1038/s41586-021-03819-2)

[Transformer]
**Accurate prediction of protein structures and interactions using a three-track neural network**   
[Baek, Minkyung, et al.Science 373.6557 (2021): 871-876.](https://doi.org/10.1126/science.abj8754)

### Classification
[RNN]
**Predictive profiling of SARS-CoV-2 variants by deep mutational learning**   
[Taft, Joseph M., et al. Available at SSRN 3982671 (2021).](https://doi.org/10.1101/2021.12.07.471580)   
- combinatorial mutagenesis of RBD
- model for ACE2 binder/non-binder; mAb escaper/non-escaper

[CNN]
**ProteInfer: deep networks for protein functional inference**   
[Sanderson, Theo, et al. bioRxiv (2021).](https://doi.org/10.1101/2021.09.20.461077)   
- function predictions ( GO terms and EC number)

[GCN+RNN]
**Structure-based protein function prediction using graph convolutional networks**   
[Gligorijević, Vladimir, et al. Nature communications 12.1 (2021): 1-14.](https://doi.org/10.1038/s41467-021-23303-9)   
- function predictions ( GO terms and EC number)
- LSTM for sequence and GCN for structure

[MLP]
**Deep learning for identifying antibody repsonse to dengue infection using CDR H3 info**   
[Horst, Alexander et al. Frontiers in Artificial Intelligence 4:715462 (2021)](https://doi.org/10.3389/frai.2021.715462)

### Predicting interactions
[geometric deep learning]
**Deciphering interaction fingerprints from protein molecular surfaces using geometric deep learning**   
[Gainza, Pablo, et al. Nature Methods 17.2 (2020): 184-192.](https://doi.org/10.1038/s41592-019-0666-6)   
- ligand pocket similarity comparison
- protein–protein interaction (PPI) site prediction
- scanning of surfaces

[geometric deep learning]
**A geometric deep learning approach to predict binding conformations of bioactive molecules**   
[Méndez-Lucio, Oscar, et al. Nature Machine Intelligence 3.12 (2021): 1033-1039.](https://doi.org/10.1038/s42256-021-00409-9)   
- statistical potential of ligand–target complex based on distance likelihood
- ligand–target binding conformation

### Generative models
[transformer/Masked-Language Modeling]
**Generative Language Modeling for Antibody Design**   
[Shuai, Richard W., Jeffrey A. Ruffolo, and Jeffrey J. Gray. bioRxiv (2021).](https://doi.org/10.1101/2021.12.13.472419)   
- train 558M antibody from OAS with (maksed token, answer) as input
- generate antibody sequence library with CDRH3 maksed

[transformer/next-token prediction]
**ProGen: Language Modeling for Protein Generation**   
[Madani, Ali, et al. arXiv preprint arXiv:2004.03497 (2020).](https://arxiv.org/abs/2004.03497)
- transformer, 280M protein sequences with (tag,sequence) as input

[GAN/CNN]
**Expanding functional protein sequence spaces using generative adversarial networks**   
[Repecka, Donatas, et al. Nature Machine Intelligence 3.4 (2021): 324-333.](https://doi.org/10.1038/s42256-021-00310-5)
- proteinGAN, 16,706 bacterial MDH enzymes as training set
- expands the known MDH sequence space, experiemtal validated


### Representation learning with self-supervised learning
[transformer/Masked-Language Modeling]
**Biological structure and function emerge from scaling unsupervised learning to 250 million protein sequences**   
[Rives, Alexander, et al. Proceedings of the National Academy of Sciences 118.15 (2021).](https://doi.org/10.1073/pnas.2016239118)
- protein language model trained on 250M protein sequences
- represent physicochemical properties and secondary structure
- mutational effect prediction

[transformer/Masked-Language Modeling]
**MSA Transformer**   
[Rao, Roshan, et al. bioRxiv (2021).](https://doi.org/10.1101/2021.02.12.430858)
- protein language model trained on 26 million MSAs
- row and column attention
- represent physicochemical properties and secondary structure; mutational effect prediction

[transformer/Masked-Language Modeling]
**Language models enable zero-shot prediction of the effects of mutations on protein function**   
[Meier, Joshua, et al. Advances in Neural Information Processing Systems 34 (2021).](https://doi.org/10.1101/2021.07.09.450648)
- protein language model trained on 98M protein sequences, Masked-Language Modeling
- score mutational effect with the predicted probability
- Zero-shot transfer, ESM-1v, mutational effect prediction

[tools from above papers]
**Pretrained language models for proteins**
[Facebook AI Research](https://github.com/facebookresearch/esm)

[RNN/next-token prediction]
**Unified rational protein engineering with sequence-based deep representation learning**   
[Alley, Ethan C., et al. Nature methods 16.12 (2019): 1315-1322.](https://doi.org/10.1038/s41592-019-0598-1)
- UniRep, mLSTM trained on 24 million UniRef50 proteins
- encodes physicochemistry, organism level information, secondary structure, evolutionary and functional information, and higher-order structural features

[transformer/Masked-Language Modeling]
**ProtTrans: Towards Cracking the Language of Lifes Code Through Self-Supervised Deep Learning and High Performance Computing**   
[Elnaggar, Ahmed, et al. bioRxiv. 2020." URL http://arxiv. org/abs (2007).](https://github.com/agemagician/ProtTrans)
- protein embeddings
- per-residue prediction of protein secondary structure
- per-protein predictions of protein sub-cellular localization
