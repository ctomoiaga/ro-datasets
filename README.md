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
| [FulG](https://huggingface.co/datasets/faur-ai/fulg) / [arXiv](https://arxiv.org/abs/2407.13657) | Used CCNet for processing | CommonCrawl filtered and processed for Romanian language |
| [FineWeb](https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1) / [Blog](https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1)| Good documentation | CommonCrawl filtering procedure and dataset for English, it can be adapted for Romanian by using datatrove |
| [OSCAR](https://oscar-project.github.io/documentation/versions/oscar-2301/) | Good CommonCrawl processing | CommonCrawl filtered and processed dataset available |
| [Readerbench](https://huggingface.co/readerbench) | Good space for Romanian datasets | Training classifiers and using already trained one |
| [CommonCrawl Statistics](https://commoncrawl.github.io/cc-crawl-statistics/plots/tld/latestcrawl.html) | Statistics of CommonCrawl

### Datasets
Some datasets are very large and are not processed ( may contain multiple languages ). Detecting Romanian language is usually easy.
Most if not all datasets are not instruct ready, additional steps are needed to add instructions

| Dataset                                                                                                       | Notes                                                                             |
| ------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | 
| [mOSCAR](https://huggingface.co/datasets/oscar-corpus/mOSCAR/viewer/ron_Latn)                                 | Multilingual OSCAR dataset, needs further processing. See additional datasets on their HF space. |
| [faur-ai/fulg](https://huggingface.co/datasets/faur-ai/fulg)                                                  | CommonCrawl filtered and processed for Romanian |
| [mC4 RO](https://huggingface.co/datasets/allenai/c4/viewer/ro)                                                | CommonCrawl the C4 version [Docs](https://github.com/allenai/c4-documentation)
| [readerbench/ro-human-machine-60k](https://huggingface.co/datasets/readerbench/ro-human-machine-60k)          | Needs further processing for instruct fine-tuning an LLM | 
| [CC-100](https://data.statmt.org/cc-100/)                                                                     | Attempt to recreate the dataset used for training XLM-R. This corpus comprises of monolingual data for 100+ languages |
| [Wikipedia RO](https://huggingface.co/datasets/wikimedia/wikipedia/viewer/20231101.ro)                        | Wikipedia, the Romanian part |
| [RoMath](https://huggingface.co/datasets/cosmadrian/romath)                                                   | I did not had the time to check it's value. A Mathematical Reasoning Benchmarking Suite from Descriptions in 🇷🇴 Romanian 🇷🇴 |

### Tools
| Link                                                         | Comments                                                                                        |
| ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------- |
| [Trafilatura](https://trafilatura.readthedocs.io/en/latest/) | Good for extracting text from web                                                               |
| [Datatrove](https://github.com/huggingface/datatrove)        | Datatrove and examples with the Fineweb pipeline, can be addapted for Ro                        |

