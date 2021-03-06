# UkrainianLT

A collection of links to Ukrainian language tools


## NEWS

* improved results for Finnish - Ukrainian
* [LDC data sets](https://www.ldc.upenn.edu/collaborations/current-projects/disaster-and-refugee-relief-research)
* New parallel data: [MultParaCrawl v9b](https://opus.nlpl.eu/MultiParaCrawl.php) and [SUMMA](https://opus.nlpl.eu/SUMMA.php) including Ukrainian
* [Added link to another list of Ukrainian NLP](https://github.com/asivokon/awesome-ukrainian-nlp)
* [Updated translation models at Huggingface](https://huggingface.co/models?language=uk&pipeline_tag=translation&sort=modified)
* [Bilingual pictograms in various languages](pictograms.md)
* [big](opus-mt-ukr-flores-devtest-big.md), [base](opus-mt-ukr-flores-devtest-base.md) and [tiny](opus-mt-ukr-flores-devtest-tiny.md) transformer models from OPUS-MT
* new translation tools with Ukrainian language support
* [updated table with new OPUS-MT models](opus-mt-ukr-flores-devtest.md) with benchmarks on flores101 scores


## Chat bots and other on-line tools

* [HelpUkraineBot](https://helpukrainebot.com/en) - Latvia’s assistance to Ukraine
* OPUS-MT Telegram Translation Bot: https://t.me/opusmt_bot
* Ukrainian - Czech Telegram Translation Bot: http://t.me/uk_cs_translation_bot
* Ukrainian - Czech Messenger Translation Bot: https://m.me/uk.cs.translation.bot
* more about translation bots: https://github.com/martin-majlis/uk-cs-translation-bot


## Translation

### On-line translation tools

* [Bergamot client-side browser-based translator](https://translatelocally.com/web/)
* [UFAL translator for Czech - Ukrainian](https://lindat.cz/translation/) ([project website](https://ufal.mff.cuni.cz/ufal-ukraine))
* [OPUS-MT web-interface](https://translate.ling.helsinki.fi/ui/ukrainian)
* [Google translate](https://translate.google.com/)
* [Microsoft Bing translator](https://www.bing.com/Translator)
* [AppTek translator](https://www.apptek.com/technology/machine-translation)
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
* [OPUS-MT-app](https://github.com/Helsinki-NLP/OPUS-MT-app/) and [translatelocally](https://translatelocally.com/) - speed-optimized local translation - now with models for Ukrainian; also available as [client-side web browser app](https://translatelocally.com/web/)


Deployable MT server solutions, web apps, docker containers:

* [OPUS-MT](https://github.com/Helsinki-NLP/OPUS-MT), basically all released [OPUS-MT](https://opus.nlpl.eu/Opus-MT/) and [Tatoeba MT models](https://github.com/Helsinki-NLP/Tatoeba-Challenge/blob/master/results/tatoeba-models-all.md) can be used
* [OPUS-MT docker containers](https://hub.docker.com/repository/docker/helsinkinlp/tatoeba-mt)


Huggingface:

* [Ukrainian Translation models](https://huggingface.co/models?language=uk&pipeline_tag=translation&sort=modified)

Example use for hf models (Ukrainian - English):

```python
from transformers import pipeline
pipe = pipeline("translation", model="Helsinki-NLP/opus-mt-tc-big-zle-en")
print(pipe("Мене звати Вольфґанґ і я живу в Берліні."))

# [{'translation_text': 'My name is Wolfgang and I live in Berlin.'}]
```


European Language Grid:

* [Machine translation at ELG](https://live.european-language-grid.eu/catalogue/search/Ukrainian?&function__term=Machine%20Translation&language__term=Ukrainian)
* [Ukrainian LT resources at the European Language Grid](https://live.european-language-grid.eu/catalogue/search/Ukrainian?language__term=Ukrainian)




### MT Data sets

* [OPUS](https://opus.nlpl.eu/), use [OPUS-API](https://opus.nlpl.eu/opusapi/) to search for resources, for example [all bitexts for English-Ukrainian](https://opus.nlpl.eu/opusapi/?source=en&target=uk&preprocessing=moses&version=latest)
* [MultParaCrawl](https://opus.nlpl.eu/MultiParaCrawl.php) - Crawled parallel corppra including Ukrainian
* [SUMMA](https://opus.nlpl.eu/SUMMA.php) - Ukrainian - English data
* [Tatoeba MT Challenge data sets](https://github.com/Helsinki-NLP/Tatoeba-Challenge/)
* [OPUS-MT-testsets, various sources](https://github.com/Helsinki-NLP/OPUS-MT-testsets)
* [Polish-Ukrainian Parallel Corpus at ELG](https://live.european-language-grid.eu/catalogue/corpus/8618)
* [Back-translated monolingual Wiki data](https://github.com/Helsinki-NLP/Tatoeba-Challenge/blob/master/data/Backtranslations.md)


Tools to handle data:

* [OPUS-tools](https://pypi.org/project/opustools/) - search and download OPUS data
* [mt-data](https://github.com/thammegowda/mtdata) - download data sets from various sources
* [OpusFilter](https://github.com/Helsinki-NLP/OpusFilter) - filter / cleanup data sets



## Speech recognition and synthesis (ASR, TTS)

* [Vosk, an open-source realtime ASR system based on Kaldi including a Ukrainian model](https://alphacephei.com/vosk/models)
* [ASR for Ukrainian at ELG](https://live.european-language-grid.eu/catalogue/tool-service/18079)
* [Links to ASR, TTS and speech resources for Ukrainian](https://github.com/egorsmkv/speech-recognition-uk)
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




## Language models

* [Ukrainian Roberta](https://huggingface.co/youscan/ukr-roberta-base)



## Linguistic tools

* [pymorph2](https://github.com/kmike/pymorphy2) - morphological analyzer for Russian and Ukrainian


## Other LT resources and links

* [LDC data sets](https://www.ldc.upenn.edu/collaborations/current-projects/disaster-and-refugee-relief-research)
* [Multilingual pictograms](pictograms.md)
* [Ukrainian LT resources at huggingface](https://huggingface.co/models?language=uk)
* [Ukrainian LT resources at the European Language Grid](https://live.european-language-grid.eu/catalogue/search/Ukrainian)
* [Resources and links collected by ELRA](https://cloud.elra.info/s/S7tCCkjyRpfLdF5)
* [Another curated list of Ukrainian NLP](https://github.com/asivokon/awesome-ukrainian-nlp)
