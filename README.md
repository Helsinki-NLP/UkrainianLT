# UkrainianLT

A collection of links to Ukrainian language tools


## Speech recognition

* [Models at huggingface](https://huggingface.co/models?language=uk&pipeline_tag=automatic-speech-recognition&sort=downloads)



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

* [Dutch - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18045)
* [English - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18040)
* [French - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18041)
* [German - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18039)
* [Hebrew - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18042)
* [Hungarian - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18043)
* [Italian - Uktainian](https://live.european-language-grid.eu/catalogue/tool-service/18044)
* [Polish - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18046)
* [Portuguese - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18047)
* [Russian - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18048)
* [Spanish - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18049)
* [Turkish - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/18050)
* [East Slavic languages - Ukrainian](https://live.european-language-grid.eu/catalogue/tool-service/9257)
* [Ukrainian - English](https://live.european-language-grid.eu/catalogue/tool-service/9216)
* [Ukrainian - Hebrew](https://live.european-language-grid.eu/catalogue/tool-service/18051)
* [Ukrainian - Hungarian](https://live.european-language-grid.eu/catalogue/tool-service/18052)
* [Ukrainian - Russian](https://live.european-language-grid.eu/catalogue/tool-service/18053)
* [Ukrainian - Turkish](https://live.european-language-grid.eu/catalogue/tool-service/18054)



### Pre-trained translation models

OPUS-MT (see also the [full list of models](https://github.com/Helsinki-NLP/Tatoeba-Challenge/blob/master/results/tatoeba-results-all.md)) (scores refer to the [Tatoeba benchmark](https://github.com/Helsinki-NLP/Tatoeba-Challenge)):

| Language Pair         | Language IDs  |  chr-F        | BLEU          | NMT model |
|-----------------------|---------------|---------------|---------------|-----------|
| Afrikaans-Ukrainian	|	afr-ukr	|	0.590	|	42.7	|	[gmw-zle/opus1m-2021-02-19](https://object.pouta.csc.fi/Tatoeba-MT-models/gmw-zle/opus1m-2021-02-19.zip) |
| Belarusian-Ukrainian	|	bel-ukr	|	0.760	|	59.5	|	[bel+rus+ukr-bel+rus+ukr/opus-2020-06-16](https://object.pouta.csc.fi/Tatoeba-MT-models/bel+rus+ukr-bel+rus+ukr/opus-2020-06-16.zip) |
| Bulgarian-Ukrainian	|	bul-ukr	|	0.690	|	50.0	|	[sla-sla/opus-2020-07-21](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-07-21.zip) |
| Catalan-Ukrainian	|	cat-ukr	|	0.545	|	32.1	|	[roa-zle/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/roa-zle/opus1m-2021-02-18.zip) |
| Czech-Ukrainian	|	ces-ukr	|	0.687	|	52.9	|	[sla-sla/opus-2020-07-27](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-07-27.zip) |
| German-Ukrainian	|	deu-ukr	|	0.612	|	40.2	|	[deu-ukr/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/deu-ukr/opus-2021-02-18.zip) |
| English-Ukrainian	|	eng-ukr	|	0.597	|	38.9	|	[eng-ukr/opus+bt-2021-04-14](https://object.pouta.csc.fi/Tatoeba-MT-models/eng-ukr/opus+bt-2021-04-14.zip) |
| French-Ukrainian	|	fra-ukr	|	0.599	|	39.3	|	[fra-ukr/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/fra-ukr/opus-2021-02-18.zip) |
| Serbo-Croatian-Ukrainian	|	hbs-ukr	|	0.689	|	51.1	|	[sla-sla/opus-2020-10-04](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-10-04.zip) |
| Hebrew-Ukrainian	|	heb-ukr	|	0.552	|	35.4	|	[heb-ukr/opus-2021-02-19](https://object.pouta.csc.fi/Tatoeba-MT-models/heb-ukr/opus-2021-02-19.zip) |
| Croatian-Ukrainian	|	hrv-ukr	|	0.654	|	45.6	|	[sla-sla/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2021-02-18.zip) |
| Hungarian-Ukrainian	|	hun-ukr	|	0.611	|	41.2	|	[hun-ukr/opus-2021-02-19](https://object.pouta.csc.fi/Tatoeba-MT-models/hun-ukr/opus-2021-02-19.zip) |
| Italian-Ukrainian	|	ita-ukr	|	0.657	|	45.9	|	[ita-ukr/opus-2021-02-19](https://object.pouta.csc.fi/Tatoeba-MT-models/ita-ukr/opus-2021-02-19.zip) |
| Dutch-Ukrainian	|	nld-ukr	|	0.619	|	40.8	|	[nld-ukr/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/nld-ukr/opus-2021-02-18.zip) |
| Norwegian-Ukrainian	|	nor-ukr	|	0.625	|	41.2	|	[nor-ukr/opus-2021-02-23](https://object.pouta.csc.fi/Tatoeba-MT-models/nor-ukr/opus-2021-02-23.zip) |
| Polish-Ukrainian	|	pol-ukr	|	0.665	|	47.1	|	[pol-ukr/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/pol-ukr/opus-2021-02-18.zip) |
| Portuguese-Ukrainian	|	por-ukr	|	0.624	|	41.2	|	[por-ukr/opus-2021-02-23](https://object.pouta.csc.fi/Tatoeba-MT-models/por-ukr/opus-2021-02-23.zip) |
| Russian-Ukrainian	|	rus-ukr	|	0.793	|	64.0	|	[rus-ukr/opus-2021-02-19](https://object.pouta.csc.fi/Tatoeba-MT-models/rus-ukr/opus-2021-02-19.zip) |
| Slovenian-Ukrainian	|	slv-ukr	|	0.551	|	36.6	|	[sla-sla/opus-2020-09-26](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-09-26.zip) |
| Spanish-Ukrainian	|	spa-ukr	|	0.614	|	41.3	|	[spa-ukr/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/spa-ukr/opus-2021-02-18.zip) |
| Serbian-Ukrainian	|	srp_Cyrl-ukr	|	0.689	|	52.3	|	[sla-sla/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2021-02-18.zip) |
| Serbian-Ukrainian	|	srp_Latn-ukr	|	0.736	|	57.1	|	[sla-sla/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2021-02-18.zip) |
| Turkish-Ukrainian	|	tur-ukr	|	0.624	|	42.5	|	[tur-ukr/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/tur-ukr/opus-2021-02-18.zip) |
| Ukrainian-Afrikaans	|	ukr-afr	|	0.722	|	55.4	|	[zle-gmw/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-gmw/opus1m-2021-02-18.zip) |
| Ukrainian-Belarusian	|	ukr-bel	|	0.719	|	51.3	|	[zle-zle/opus-2020-07-27](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-zle/opus-2020-07-27.zip) |
| Ukrainian-Bulgarian	|	ukr-bul	|	0.732	|	56.6	|	[sla-sla/opus-2020-10-04](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-10-04.zip) |
| Ukrainian-Catalan	|	ukr-cat	|	0.598	|	39.6	|	[zle-roa/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-roa/opus1m-2021-02-18.zip) |
| Ukrainian-Czech	|	ukr-ces	|	0.686	|	52.1	|	[sla-sla/opus-2020-07-27](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-07-27.zip) |
| Ukrainian-German	|	ukr-deu	|	0.672	|	50.0	|	[zle-gmw/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-gmw/opus1m-2021-02-18.zip) |
| Ukrainian-English	|	ukr-eng	|	0.70441	|	55.8	|	[zle-eng/opusTCv20210807+bt_transformer-big_2022-03-03](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-eng/opusTCv20210807+bt_transformer-big_2022-03-03.zip) |
| Ukrainian-Esperanto	|	ukr-epo	|	0.562	|	34.2	|	[tatoeba-zero/opus-2020-06-21](https://object.pouta.csc.fi/Tatoeba-MT-models/tatoeba-zero/opus-2020-06-21.zip) |
| Ukrainian-French	|	ukr-fra	|	0.644	|	47.3	|	[zle-roa/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-roa/opus1m-2021-02-18.zip) |
| Ukrainian-Serbo-Croatian	|	ukr-hbs	|	0.671	|	47.2	|	[sla-sla/opus-2020-10-04](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-10-04.zip) |
| Ukrainian-Hebrew	|	ukr-heb	|	0.557	|	35.7	|	[ukr-heb/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/ukr-heb/opus-2021-02-18.zip) |
| Ukrainian-Croatian	|	ukr-hrv	|	0.664	|	47.4	|	[sla-sla/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2021-02-18.zip) |
| Ukrainian-Hungarian	|	ukr-hun	|	0.649	|	41.4	|	[ukr-hun/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/ukr-hun/opus-2021-02-18.zip) |
| Ukrainian-Italian	|	ukr-ita	|	0.671	|	46.4	|	[zle-roa/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-roa/opus1m-2021-02-18.zip) |
| Ukrainian-Dutch	|	ukr-nld	|	0.670	|	50.4	|	[zle-gmw/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-gmw/opus1m-2021-02-18.zip) |
| Ukrainian-Norwegian	|	ukr-nor	|	0.699	|	55.0	|	[ukr-nor/opus-2021-02-24](https://object.pouta.csc.fi/Tatoeba-MT-models/ukr-nor/opus-2021-02-24.zip) |
| Ukrainian-Polish	|	ukr-pol	|	0.695	|	50.1	|	[sla-sla/opus-2020-07-27](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2020-07-27.zip) |
| Ukrainian-Portuguese	|	ukr-por	|	0.612	|	39.8	|	[zle-roa/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-roa/opus1m-2021-02-18.zip) |
| Ukrainian-Russian	|	ukr-rus	|	0.826	|	69.2	|	[ukr-rus/opus-2021-02-19](https://object.pouta.csc.fi/Tatoeba-MT-models/ukr-rus/opus-2021-02-19.zip) |
| Ukrainian-Spanish	|	ukr-spa	|	0.662	|	47.6	|	[zle-roa/opus1m-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/zle-roa/opus1m-2021-02-18.zip) |
| Ukrainian-Serbian	|	ukr-srp_Cyrl	|	0.683	|	51.4	|	[sla-sla/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2021-02-18.zip) |
| Ukrainian-Serbian	|	ukr-srp_Latn	|	0.671	|	43.5	|	[sla-sla/opus-2021-02-18](https://object.pouta.csc.fi/Tatoeba-MT-models/sla-sla/opus-2021-02-18.zip) |
| Ukrainian-Turkish	|	ukr-tur	|	0.655	|	39.3	|	[ukr-tur/opus-2021-02-19](https://object.pouta.csc.fi/Tatoeba-MT-models/ukr-tur/opus-2021-02-19.zip) |


### MT Data sets

* [OPUS](https://opus.nlpl.eu/), use [OPUS-API](https://opus.nlpl.eu/opusapi/) to search for resources, for example [all bitexts for English-Ukrainian](https://opus.nlpl.eu/opusapi/?source=en&target=uk&preprocessing=moses&version=latest)
* [Tatoeba MT Challenge data sets](https://github.com/Helsinki-NLP/Tatoeba-Challenge/)
* [OPUS-MT-testsets, various sources](https://github.com/Helsinki-NLP/OPUS-MT-testsets)


Tools to handle data:

* [OPUS-tools](https://pypi.org/project/opustools/) - search and download OPUS data
* [mt-data](https://github.com/thammegowda/mtdata) - download data sets from various sources
* [OpusFiler](https://github.com/Helsinki-NLP/OpusFilter) - filter / cleanup data sets



## Language models

* [Ukrainian Roberta](https://huggingface.co/youscan/ukr-roberta-base)


## Other LT resources and links

* [Ukrainian LT resources at huggingface](https://huggingface.co/models?language=uk)
* [Ukrainian LT resources at the European Language Grid](https://live.european-language-grid.eu/catalogue/search/Ukrainian)
