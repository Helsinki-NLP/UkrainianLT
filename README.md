# UkrainianLT

A collection of links to Ukrainian language tools


## NEWS

* new translation tools with Ukrainian language support
* moved MT model list to separate pages
* updated table with new OPUS-MT models
* benchmarks on flores101 scores


## Speech recognition and synthesis (ASR, TTS)

* [ASR for Ukrainian at ELG](https://live.european-language-grid.eu/catalogue/tool-service/18079)
* [Models at huggingface](https://huggingface.co/models?language=uk&pipeline_tag=automatic-speech-recognition&sort=downloads)

Resources from ELRA, may be provided free of charge. Please contact info@elda.org:

* http://catalog.elra.info/en-us/repository/browse/ELRA-S0043/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0377/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0378/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0399/
* http://catalog.elra.info/en-us/repository/browse/ELRA-S0400/
* [more info](https://cloud.elra.info/s/S7tCCkjyRpfLdF5?path=%2FSpeech%20resources)

Resources from ELG:

* [GlobalPhone Ukrainian](https://live.european-language-grid.eu/catalogue/corpus/1481)
* [GlobalPhone Ukrainian Pronunciation Dictionary](https://live.european-language-grid.eu/catalogue/lcr/2218)


## Translation

### On-line translation tools

* [Bergamot client-side browser-based translator](https://translatelocally.com/web/)
* [OPUS-MT web-interface](https://translate.ling.helsinki.fi/ui/ukrainian)
* [Google translate](https://translate.google.com/)
* [Microsoft Bing translator](https://www.bing.com/Translator)
* [Tilde trainslator](https://translate.tilde.com)

### Pre-trained translation models

* [Best OPUS-MT models for Ukrainian evaluated on the flores101 devtest benchmark](opus-mt-ukr-flores-devtest.md)
* [Tiny Transformer OPUS-MT models for Ukrainian evaluated on the flores101 devtest benchmark](opus-mt-ukr-flores-devtest-tiny.md)
* [Base Transformer OPUS-MT models for Ukrainian evaluated on the flores101 devtest benchmark](opus-mt-ukr-flores-devtest-base.md)
* [Big Transformer OPUS-MT models for Ukrainian evaluated on the flores101 devtest benchmark](opus-mt-ukr-flores-devtest-big.md)
* [Full list of OPUS-MT models](https://github.com/Helsinki-NLP/Tatoeba-Challenge/blob/master/results/tatoeba-results-all.md)



### Translation APIs / deployable containers / workflow integration

Computer-aided translation / interactive translation:

* [OPUS-CAT](https://helsinki-nlp.github.io/OPUS-CAT/): plugins for common translation tools, downloadable MT models from OPUS-MT
* [OPUS-MT-app (translateLocally)](https://github.com/Helsinki-NLP/OPUS-MT-app/) - speed-optimized local translation - now with models for Ukrainian to English and English to Ukrainian (NOTE: models are broken on Windows, unfortunately!)


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

* [Machine translation at ELG](https://live.european-language-grid.eu/catalogue/search/Ukrainian?&function__term=Machine%20Translation&language__term=Ukrainian)
* [Ukrainian LT resources at the European Language Grid](https://live.european-language-grid.eu/catalogue/search/Ukrainian?language__term=Ukrainian)




### MT Data sets

* [OPUS](https://opus.nlpl.eu/), use [OPUS-API](https://opus.nlpl.eu/opusapi/) to search for resources, for example [all bitexts for English-Ukrainian](https://opus.nlpl.eu/opusapi/?source=en&target=uk&preprocessing=moses&version=latest)
* [Tatoeba MT Challenge data sets](https://github.com/Helsinki-NLP/Tatoeba-Challenge/)
* [OPUS-MT-testsets, various sources](https://github.com/Helsinki-NLP/OPUS-MT-testsets)
* [Polish-Ukrainian Parallel Corpus at ELG](https://live.european-language-grid.eu/catalogue/corpus/8618)
* [Back-translated monolingual Wiki data](https://github.com/Helsinki-NLP/Tatoeba-Challenge/blob/master/data/Backtranslations.md)


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
