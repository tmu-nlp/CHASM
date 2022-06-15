
[![](https://img.shields.io/badge/license-CC%20BY--NC--SA-green)](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode.txt)

# CHASM: A Corpus of Countering HAte Speech and Microaggressions
This is a repository for the corpus of Countering HAte Speech and Microaggressions (CHASM).
CHASM is pronounced /ˈkæzəm/, as in "Crossing the Chasm."

## About CHASM
The CHASM dataset contains: 
- 306 counterspeech and 42 microintervention messages generated by GPT-2, GPT-Neo, and GPT-3 using prompting 
- labels obtained through human evaluation on Amazon Mechanical Turk:
  - offensiveness of each hate speech or microaggressions
  - offensiveness, stance, and informativeness of each model's generation

## Dataset
* `counter_conan.json`
* `counter_sbic.json`

### Formats

The formats of each dataset:

* `id`: id for a set of the four sentences
  * `post`
    * `text`: hate speech or microaggressions
    * `score`: a list of scores for **offensiveness** annotated by crowdworkers, a total of nine labels (three workers per each of the three models)
  * `GPT-3`:
    * `text`: counternarrative
    * `score`: 
      * `off`: a list of scores for **offensiveness** annotated by three crowdworkers
      * `stance`: a list of scores for **stance** annotated by three crowdworkers
      * `info`: a list of scores for **informativeness** annotated by three crowdworkers
  * `GPT-2` has the fields `text` and `score` as in `GPT-3`
  * `GPT-Neo` has the fields `text` and `score` as in `GPT-3`

## Citation

Mana Ashida and Mamoru Komachi. Towards Automatic Generation of Messages Countering Online Hate Speech and Microaggressions. The 6th Workshop on Online Abuse and Harms (WOAH) 2022. (to appear)


Please also cite following [CONAN](https://github.com/marcoguerini/CONAN) datasets (link to github repo):
```
@inproceedings{chung-etal-2019-conan,
    title = "{CONAN} - {CO}unter {NA}rratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech",
    author = "Chung, Yi-Ling and Kuzmenko, Elizaveta and Tekiroglu, Serra Sinem and Guerini, Marco",
    booktitle = "Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics",
    month = jul,
    year = "2019",
    address = "Florence, Italy",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/P19-1271",
    doi = "10.18653/v1/P19-1271",
    pages = "2819--2829"
}
```
```
@inproceedings{fanton-2021-human,
  title="{Human-in-the-Loop for Data Collection: a Multi-Target Counter Narrative Dataset to Fight Online Hate Speech}",
  author="{Fanton, Margherita and Bonaldi, Helena and Tekiroğlu, Serra Sinem and Guerini, Marco}",
  booktitle = "Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics",
  month = aug,
  year = "2021",
  publisher = "Association for Computational Linguistics",
}
```
```
@inproceedings{chung-etal-2021-knowledge,
    title = "{Towards Knowledge-Grounded Counter Narrative Generation for Hate Speech",
    author = "Chung, Yi-Ling and Tekiroğlu, Serra Sinem and Guerini, Marco",
    booktitle = "Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics",
    month = aug,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
}
```
As well as [SBIC](https://aclanthology.org/2020.acl-main.486/) and [SelfMA](https://aclanthology.org/D19-1176/) dataset (link to paper)
```
@inproceedings{sap2020socialbiasframes,
   title={Social Bias Frames: Reasoning about Social and Power Implications of Language},
   author={Sap, Maarten and Gabriel, Saadia and Qin, Lianhui and Jurafsky, Dan and Smith, Noah A and Choi, Yejin},
   year={2020},
   booktitle={ACL},
}
```

```
@inproceedings{breitfeller-etal-2019-finding,
    title = "Finding Microaggressions in the Wild: A Case for Locating Elusive Phenomena in Social Media Posts",
    author = "Breitfeller, Luke  and
      Ahn, Emily  and
      Jurgens, David  and
      Tsvetkov, Yulia",
    booktitle = "Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP)",
    month = nov,
    year = "2019",
    address = "Hong Kong, China",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/D19-1176",
    doi = "10.18653/v1/D19-1176",
    pages = "1664--1674",
    abstract = "Microaggressions are subtle, often veiled, manifestations of human biases. These uncivil interactions can have a powerful negative impact on people by marginalizing minorities and disadvantaged groups. The linguistic subtlety of microaggressions in communication has made it difficult for researchers to analyze their exact nature, and to quantify and extract microaggressions automatically. Specifically, the lack of a corpus of real-world microaggressions and objective criteria for annotating them have prevented researchers from addressing these problems at scale. In this paper, we devise a general but nuanced, computationally operationalizable typology of microaggressions based on a small subset of data that we have. We then create two datasets: one with examples of diverse types of microaggressions recollected by their targets, and another with gender-based microaggressions in public conversations on social media. We introduce a new, more objective, criterion for annotation and an active-learning based procedure that increases the likelihood of surfacing posts containing microaggressions. Finally, we analyze the trends that emerge from these new datasets.",
}
```

## Contact

Mana ASHIDA, maashida@yahoo-corp.jp
