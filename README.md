# Advanced NLP –  Project 

## About
This repository consists of experiements conducted on Sarcasm and Irony datasets using various model architectures.
The quality of the language model is measured through confusion matrix

## Project files
### Common Util files
<li>preprocessing.ipynb module consists of various methods to load datasets, generate datasets, applying tokenization, etc</li>
<li>It consists of various cleaning methods to clean the text like following:
<ol>
<li> replace_url to replace urls with URL </li>
<li> replace_hashtags to replace with HASHTAG </li>
<li>  replace_email to replace with EMAIL </li>
<li>  replace_mentions to replace with MENTION </li>
<li>  replace_numbers to replace with NUMBER </li>
<li>  remove_abbrevations to replace possessive words with their extended representations.</li>
<li>  remove_special_patterns to replace words like 10334m delimiter words found in corpus.</li>
<li>  remove_punctuation to remove the punctuations and it can be replaced with PUNCT </li></ol></li>

#### Transformers specific preprocessing
<li>
Since transformers are powered by powerful tokenization like BPE etc, we restrcited preprocessing to following:
<ol>
<li>replace_url to replace urls with URL</li>
<li>Include special token '[EMOTICON]' for the sentence where emoticons and text baesd smilies are present</li>
<li>Include special token '[ELONGATED]' for the sentences where words with elongaged expressions present like "foreveeer", "yayyy", "Aweeeeesome", etc</li>
</ol>
</li>

### Model specific files
<li>experiment/Irony_bilstm.ipynb consists of training code and evaluation loop methods for Bilstm model with attention </li>
<li>experiment/irony_transformers_hf.ipynb consists of bidirectional encoder transformer model implementation</li>
<li>experiment/irony_transformers_torch.ipynb consists of transformer encoder model implementation</li>
<li>experiment/setfit_impl.ipynb consists of setfit few shot training implementation</li>
<li>experiment/setfit_impl.ipynb consists of setfit few shot training implementation</li>
<li>experiment/irony_tf_exponential.ipynb consists of exponential task specific postional encoding transformer training implementation</li>

### Troubleshooting
Often times the execution may fail if python path is not set correctly.
Try loading the project to IDE for smooth execution.

### Contact
Contact author for any queries to reproduce the results


