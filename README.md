<div align="center">
  <h1> 🇷🇴 RO LLM Datasets and Tools </h1>
  <p>
    🤗 <a href="https://huggingface.co/chrisgru">Hugging Face</a> • 
  </p>
   <p><em>List of datasets, tools and procedures to help anyone training LLMs and other types of models related to the Romanian language</em></p>
</div>
<br/>

### Links
| Links                         |  Comments                      | Description                                                                                                               | 
| ----------------------------- | -------------------------------| ------------------------------------------------------------------------------------------------------------------------- |
| [OpenLLM-RO](https://huggingface.co/OpenLLM-Ro) / [Github](https://github.com/OpenLLM-Ro) | Most datsets are translated which leads to lower quality models | Romanian community that builds open Romanian models and tries to collect these models in a single place. |
| [FulG](https://huggingface.co/datasets/faur-ai/fulg) / [arXiv](https://arxiv.org/abs/2407.13657) | Used CCNet for processing | CommonCrawl filtered and processed for Romanian language |
| [FineWeb](https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1) / [Blog](https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1)| Good documentation | CommonCrawl filtering procedure and dataset for English, it can be adapted for Romanian by using datatrove |
| [OSCAR](https://oscar-project.github.io/documentation/versions/oscar-2301/) | Good CommonCrawl processing | CommonCrawl filtered and processed dataset available |
| [Readerbench](https://huggingface.co/readerbench) | Good space for Romanian datasets | Training classifiers and using already trained one |
| [CommonCrawl Statistics](https://commoncrawl.github.io/cc-crawl-statistics/plots/tld/latestcrawl.html) | Statistics of CommonCrawl |

### Datasets
Some datasets are very large and are not processed ( may contain multiple languages ). Detecting Romanian language is usually easy.
Most if not all datasets are not instruct ready, additional steps are needed to add instructions

| Dataset                                                                                                       | Notes                                                                             |
| ------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | 
| [OpenLLM-RO](https://huggingface.co/OpenLLM-Ro)                                                               | A lot of interesting datasets ( even if they are translations ) including fined-tuned LLMs |
| [mOSCAR](https://huggingface.co/datasets/oscar-corpus/mOSCAR/viewer/ron_Latn)                                 | Multilingual OSCAR dataset, needs further processing. See additional datasets on their HF space. |
| [faur-ai/fulg](https://huggingface.co/datasets/faur-ai/fulg)                                                  | CommonCrawl filtered and processed for Romanian |
| [mC4 RO](https://huggingface.co/datasets/allenai/c4/viewer/ro)                                                | CommonCrawl the C4 version [Docs](https://github.com/allenai/c4-documentation)
| [PleIAs/common_corpus](https://huggingface.co/datasets/PleIAs/common_corpus)                                  | Common Corpus is the largest open and permissible licensed text dataset, comprising over 2 trillion tokens (2,003,039,184,047 tokens). It is a diverse dataset, consisting of books, newspapers, scientific articles, government and legal documents, code, and more. |
| [readerbench/ro-human-machine-60k](https://huggingface.co/datasets/readerbench/ro-human-machine-60k)          | Needs further processing for instruct fine-tuning an LLM | 
| [CC-100](https://data.statmt.org/cc-100/)                                                                     | Attempt to recreate the dataset used for training XLM-R. This corpus comprises of monolingual data for 100+ languages |
| [Wikipedia RO](https://huggingface.co/datasets/wikimedia/wikipedia/viewer/20231101.ro)                        | Wikipedia, the Romanian part |
| [cosmadrian/romath](https://huggingface.co/datasets/cosmadrian/romath)                                                   | I did not had the time to check it's value. A Mathematical Reasoning Benchmarking Suite from Descriptions in 🇷🇴 Romanian 🇷🇴 |
| [cosmadrian/rocode](https://huggingface.co/datasets/cosmadrian/rocode)                                        | Small, but useful. RoCode: A Dataset for Measuring Code Intelligence from Problem Definitions in Romanian |
| [BlackKakapo](https://huggingface.co/datasets/BlackKakapo/paraphrase-ro)                                      | Multiple datasets, including instruct ones Ex: [qaworld-ro](BlackKakapo/qaworld-ro) |
| [RoITD](https://huggingface.co/datasets/dragosnicolae555/RoITD)                                               | Romanian IT Dataset (RoITD) resembling SQuAD 1.1. RoITD consists of 9575 Romanian QA pairs formulated by crowd workers. QA pairs are based on 5043 articles from Romanian Wikipedia articles describing IT and household products. |
| [30K-Romanian-Captions](https://huggingface.co/datasets/vladman-25/flickr-30k-romanian-captions)              | This dataset is a translation in romanian of the flickr 30k captions dataset |
| [Ro-STS & Others](https://huggingface.co/dumitrescustefan)                                                    | Some datasets are translated, including RO-STS. RO-STS - the Semantic Textual Similarity dataset for the Romanian language | 
| [Romanian Emotion Dataset](https://huggingface.co/datasets/Alegzandra/REDv2)                                 | The second version of the Romanian Emotions Dataset (RED) containing 5449 tweets annotated in a multi-label fashion with the following 7 emotions: Anger (Furie), Fear (Frică), Joy (Bucurie), Sadness (Tristețe), Surprise (Surpriză), Trust (Încredere) and Neutral (Neutru). |
| [lavi13/wiki_qa_instructions_ro](https://huggingface.co/datasets/lavi13/wiki_qa_instructions_ro)              | Randomly selected ~10k set of entries from the Wikipedia dataset and Mixtral 8x7B to extract Q&A pairs  |





### Tools
| Link                                                         | Comments                                                                                        |
| ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------- |
| [Trafilatura](https://trafilatura.readthedocs.io/en/latest/) | Good for extracting text from web                                                               |
| [Datatrove](https://github.com/huggingface/datatrove)        | Datatrove and examples with the Fineweb pipeline, can be addapted for Ro                        |

