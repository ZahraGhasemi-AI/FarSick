# FarSick: A Persian Semantic Textual Similarity And Natural Language Inference Dataset

This is FarSick Corpus; A Persian Semantic Textual Similarity And Natural Language Inference Dataset.

If you use this corpus, please cite this paper:
	
	Z. Ghasemi and M. A. Keyvanrad, "FarSick: A Persian Semantic Textual Similarity And Natural Language Inference Dataset," 2021 11th International Conference on Computer Engineering and Knowledge (ICCKE), 2021, pp. 194-199, doi: 10.1109/ICCKE54056.2021.9721521.
	
	@INPROCEEDINGS{9721521,
  		author={Ghasemi, Zahra and Keyvanrad, Mohammad Ali},
  		booktitle={2021 11th International Conference on Computer Engineering and Knowledge (ICCKE)},
  		title={FarSick: A Persian Semantic Textual Similarity And Natural Language Inference Dataset},
  		year={2021},
  		volume={},
  		number={},
  		pages={194-199},
  		doi={10.1109/ICCKE54056.2021.9721521}}
		
Contact:      zghasemik@gmail.com       
Project page: https://github.com/ZahraGhasemi-AI/FarSick

FarSick is the first relatively large-scale STS dataset for Persian language. It consists of about 10,000 English sentence pairs.
Each sentence pair is annotated for relatedness and semantics in meaning and for the entailment relation between the two elements.
This dataset is collected by translating and editing the sentences of SICK dataset.

- File Structure: tab-separated text file

Fields:

- pair_ID: sentence pair ID

- sentence_A: sentence A

- sentence_B: sentence B

- entailment_label: textual entailment gold label (NEUTRAL, ENTAILMENT, or CONTRADICTION)

- relatedness_score: semantic relatedness gold score (on a 1-5 continuous scale)

- entailment_AB: entailment for the A-B order (A_neutral_B, A_entails_B, or A_contradicts_B)

- entailment_BA: entailment for the B-A order (B_neutral_A, B_entails_A, or B_contradicts_A)

- sentence_A_dataset: dataset from which the original sentence A was extracted (FLICKR vs. SEMEVAL)

- sentence_B_dataset: dataset from which the original sentence B was extracted (FLICKR vs. SEMEVAL)

- SemEval_set: set including the sentence pair in SemEval 2014 Task 1 (TRIAL, TRAIN, or TEST)

- binary_label: semantic gold score (0 vs. 1)

Staistics:

- Training pairs: 4439
- Trial pairs: 495
- Test pairs: 4906
- Total pairs: 9840

- Train labels: {'entailment': 1274, 'neutral': 2524, 'contradiction': 641}, {'0': 1065, '1': 3374}
- Trial labels: {'entailment': 143, 'neutral': 281, 'contradiction': 71}, {'0': 105, '1': 390}
- Test labels: {'entailment': 1404, 'neutral': 2790, 'contradiction': 712} {'0':1126, '1':3780}

- Training number of tokens: 3384
- Trial number of tokens: 1264
- Test number of tokens: 3360
