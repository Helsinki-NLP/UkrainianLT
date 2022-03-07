# UkrainianLT

A collection of links to Ukrainian language tools


## NEWS

* moved MT model list to separate pages
* updated table with new OPUS-MT models
* benchmarks on flores101 scores


## Speech recognition and synthesis (ASR, TTS)

* [Models at huggingface](https://huggingface.co/models?language=uk&pipeline_tag=automatic-speech-recognition&sort=downloads)

Resources from ELRA, may be provided free of charge. Please contact info@elda.org:

* http://catalog.elra.info/en-us/repository/browse/ELRA-S0043/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0377/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0378/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0399/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0400/
* [more info](https://cloud.elra.info/s/S7tCCkjyRpfLdF5?path=%2FSpeech%20resources)



## Translation

### On-line translation tools

* [Google translate](https://translate.google.com/)
* [OPUS-MT web-interface](https://translate.ling.helsinki.fi/ui/ukrainian)


### Translation APIs / deployable containers / workflow integration

Computer-aided translation:

* [OPUS-CAT](https://helsinki-nlp.github.io/OPUS-CAT/): plugins for common translation tools, downloadable MT models from OPUS-MT


Deployable MT server solutions, web apps, docker containers:

* [OPUS-MT](https://github.com/Helsinki-NLP/OPUS-MT), basically all released [OPUS-MT](https://opus.nlpl.eu/Opus-MT/) and [Tatoeba MT models](https://github.com/Helsinki-NLP/Tatoeba-Challenge/blob/master/results/tatoeba-models-all.md) can be used
* [OPUS-MT docker containers](https://hub.docker.com/repository/docker/helsinkinlp/tatoeba-mt)


Huggingface:

* [Ukrainian Translation models](https://huggingface.co/models?language=uk&pipeline_tag=translation&sort=downloads)

Example use for hf models (Ukrainian - English):

```python
from transformers import pipeline
pipe = pipeline("translation", model="Helsinki-NLP/opus-mt-uk-en")
print(pipe("Мене звати Вольфґанґ і я живу в Берліні."))

# [{'translation_text': 'My name is Wolfgang, and I live in Berlin.'}]
```


European Language Grid:

* [OPUS-MT models at ELG](opus-mt-ukr-elg.md)
* [Ukrainian LT resources at the European Language Grid](https://live.european-language-grid.eu/catalogue/search/Ukrainian)



### Pre-trained translation models

* [OPUS-MT models for Ukrainian evaluated on the Tatoeba benchmark](opus-mt-ukr-tatoeba.md)
* [OPUS-MT models for Ukrainian evaluated on the flores101 devtest benchmark](opus-mt-ukr-flores-devtest.md)
* [Full list of OPUS-MT models](https://github.com/Helsinki-NLP/Tatoeba-Challenge/blob/master/results/tatoeba-results-all.md)



### MT Data sets

* [OPUS](https://opus.nlpl.eu/), use [OPUS-API](https://opus.nlpl.eu/opusapi/) to search for resources, for example [all bitexts for English-Ukrainian](https://opus.nlpl.eu/opusapi/?source=en&target=uk&preprocessing=moses&version=latest)
* [Tatoeba MT Challenge data sets](https://github.com/Helsinki-NLP/Tatoeba-Challenge/)
* [OPUS-MT-testsets, various sources](https://github.com/Helsinki-NLP/OPUS-MT-testsets)


Tools to handle data:

* [OPUS-tools](https://pypi.org/project/opustools/) - search and download OPUS data
* [mt-data](https://github.com/thammegowda/mtdata) - download data sets from various sources
* [OpusFilter](https://github.com/Helsinki-NLP/OpusFilter) - filter / cleanup data sets



## Language models

* [Ukrainian Roberta](https://huggingface.co/youscan/ukr-roberta-base)



## Linguistic tools

* [pymorph2](https://github.com/kmike/pymorphy2) - morphological analyzer for Russian and Ukrainian


## Other LT resources and links

* [Ukrainian LT resources at huggingface](https://huggingface.co/models?language=uk)
* [Ukrainian LT resources at the European Language Grid](https://live.european-language-grid.eu/catalogue/search/Ukrainian)
* [Resources and links collected by ELRA](https://cloud.elra.info/s/S7tCCkjyRpfLdF5)
