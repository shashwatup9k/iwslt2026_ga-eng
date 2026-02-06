# Irish-English Speech Translation Shared Task Data@IWSLT-2025

# Introduction
Irish (also known as Gaeilge) has around 170,000 L1 speakers and “1.85 million (37%) people across the island (of Ireland) claim to be at least somewhat proficient with the language”. In the Republic of Ireland, it is the national and first official language. It is also one of the official languages of the European Union and a recognized minority language in Northern Ireland with the ISO ``ga`` code.

The IWSLT 2025 participants may obtain the Irish-English speech translation data from [here](https://github.com/shashwatup9k/iwslt2025_ga-en). The participants may also obtain following synthetic data: [Wikimedia-Speech-Irish](https://huggingface.co/datasets/ymoslem/Wikimedia-Speech-Irish), [Tatoeba](https://huggingface.co/datasets/ymoslem/Tatoeba-Speech-Irish), [EUbookshop](https://huggingface.co/datasets/ymoslem/EUbookshop-Speech-Irish). The audio data consists of the news domain, [common voice](https://commonvoice.mozilla.org/en), [Idlak](https://github.com/Idlak/Living-Audio-Dataset), and books. This corpus consists of approximately 206 hours (including synthetic data) of audio speech data and translations into English text.

We point participants to additional Irish pre-trained models (the models are trained on a common voice dataset), parallel and monolingual corpora from here:

- [wav2vec 2.0/wav2vec 2.0 (XLSR) ](https://github.com/facebookresearch/fairseq/tree/main/examples/wav2vec#pre-trained-models)
- [Opus Irish-English parallel and monolingual dataset](https://opus.nlpl.eu/results/ga&en/corpus-result-table)
- [Irish-English and English-Irish parallel COVID dataset](https://github.com/loresmt/loresmt-2021)
- [Whisper Medium GA-EN Speech Translation](https://huggingface.co/ymoslem/whisper-medium-ga2en-v6.3.0-4k-r)

**NB!** The training dataset has duplicate segments due to gender and age variety. The IWSLT 2025 test set will be available on April 01, 2025.

[April 2025 Update:] THE TEST DATA FOR 2025 IS NOW AVAILABLE [HERE](https://github.com/shashwatup9k/iwslt2025_ga-eng/tree/main/test-2025)


## Structure of the ` Shared Task data`:
```
ga-eng-iwslt2025/
├─ data/
│  ├─ IWSLT-2023 and 2024/
│  	├─ train/
│     	   └─ stamped.tsv
│     	└─ txt/
│	   └─ train.eng
│     	└─ wav/
│  	├─ dev/
│     	   └─ stamped.tsv
│     	   └─ txt/
│             └─ dev.eng
│     	   └─ wav/
│  	├─ test-2023/
│     	   └─ stamped.tsv
│     	   └─ txt/
│           └─ test.eng
│     	   └─ wav
│  	├─ test-2024/
│     	   └─ stamped.tsv
│     	   └─ txt/
│           └─ test.eng
│     	   └─ wav
│  ├─ train-2025 (Synthetic Data)/
│     └─ Wikimedia-Speech-Irish
│     └─ Tatoeba
│     └─ EUbookshop
│  ├─ test-2025 (TBD)/
│     └─ stamped.tsv
│     └─ wav/
├─ LICENSE.md
├─ README.md
   
```
The latest data statistics are presented below:
-----------------------------------------------------
```
│ Language	       			|Total_audios | Total_translatedSentences 	│ 
│IWSLT-2023 & 2024 Irish↔English (train) │  7478       │  7478            		│
│IWSLT-2023 & 2024 Irish↔English (dev)   │  1120       │  1120           		│
│IWSLT-2023 & 2024 Irish↔English (test)  │  961        │  961        			│
│Synthetic data                          │   -         |  86324                           |
│Irish↔English (test-2025)  		│  770        │  770				│
```

# License
Please see the [LICENSE](https://github.com/shashwatup9k/iwslt2025_ga-en/blob/main/LICENSE) file.

# Acknowledgments
We would like to thank [Taighde Éireann – Research Ireland](https://www.researchireland.ie/) [(grant number SFI/12/RC/2289_ P2 Insight _ 2)](https://www.insight-centre.org/). We would also like to thank RTÉ/TG4 for providing the Irish-English speech data.
## Citation
## References
<pre>
   @inproceedings{agostinelli-etal-2025-findings,
    title = "Findings of the {IWSLT} 2025 Evaluation Campaign",
    author = {Abdulmumin, Idris  and
      Agostinelli, Victor  and
      Alum{\"a}e, Tanel  and
      Anastasopoulos, Antonios  and
      Bentivogli, Luisa  and
      Bojar, Ond{\v{r}}ej  and
      Borg, Claudia  and
      Bougares, Fethi  and
      Cattoni, Roldano  and
      Cettolo, Mauro  and
      Chen, Lizhong  and
      Chen, William  and
      Dabre, Raj  and
      Est{\`e}ve, Yannick  and
      Federico, Marcello  and
      Fishel, Mark  and
      Gaido, Marco  and
      Javorsk{\'y}, D{\'a}vid  and
      Kasztelnik, Marek  and
      Kponou, Fortun{\'e}  and
      Krubi{\'n}ski, Mateusz  and
      Kin Lam, Tsz  and
      Liu, Danni  and
      Matusov, Evgeny  and
      Kumar Maurya, Chandresh  and
      P. McCrae, John  and
      Mdhaffar, Salima  and
      Moslem, Yasmin  and
      Murray, Kenton  and
      Nakamura, Satoshi  and
      Negri, Matteo  and
      Niehues, Jan  and
      Kr. Ojha, Atul  and
      Ortega, John E.  and
      Papi, Sara  and
      Pecina, Pavel  and
      Pol{\'a}k, Peter  and
      Po{\l}e{\'c}, Piotr  and
      Sankar, Ashwin  and
      Savoldi, Beatrice  and
      Sethiya, Nivedita  and
      Sikasote, Claytone  and
      Sperber, Matthias  and
      St{\"u}ker, Sebastian  and
      Sudoh, Katsuhito  and
      Thompson, Brian  and
      Turchi, Marco  and
      Waibel, Alex  and
      Wilken, Patrick  and
      Zevallos, Rodolfo  and
      Zouhar, Vil{\'e}m  and
      Z{\"u}fle, Maike},
    editor = "Salesky, Elizabeth  and
      Federico, Marcello  and
      Anastasopoulos, Antonis",
    booktitle = "Proceedings of the 22nd International Conference on Spoken Language Translation (IWSLT 2025)",
    month = jul,
    year = "2025",
    address = "Vienna, Austria (in-person and online)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.iwslt-1.44/",
    doi = "10.18653/v1/2025.iwslt-1.44",
    pages = "412--481",
    ISBN = "979-8-89176-272-5",
    abstract = "This paper presents the outcomes of the shared tasks conducted at the 22nd International Workshop on Spoken Language Translation (IWSLT). The workshop addressed seven critical challenges in spoken language translation: simultaneous and offline translation, automatic subtitling and dubbing, model compression, speech-to-speech translation, dialect and low-resource speech translation, and Indic languages. The shared tasks garnered significant participation, with 32 teams submitting their runs. The field{'}s growing importance is reflected in the increasing diversity of shared task organizers and contributors to this overview paper, representing a balanced mix of industrial and academic institutions. This broad participation demonstrates the rising prominence of spoken language translation in both research and practical applications."
}
</pre>
<pre>
   @inproceedings{ahmad-etal-2024-findings,
    title = "{FINDINGS} {OF} {THE} {IWSLT} 2024 {EVALUATION} {CAMPAIGN}",
    author = {Ahmad, Ibrahim Said  and
      Anastasopoulos, Antonios  and
      Bojar, Ond{\v{r}}ej  and
      Borg, Claudia  and
      Carpuat, Marine  and
      Cattoni, Roldano  and
      Cettolo, Mauro  and
      Chen, William  and
      Dong, Qianqian  and
      Federico, Marcello  and
      Haddow, Barry  and
      Javorsk{\'y}, D{\'a}vid  and
      Krubi{\'n}ski, Mateusz  and
      Kim Lam, Tsz  and
      Ma, Xutai  and
      Mathur, Prashant  and
      Matusov, Evgeny  and
      Maurya, Chandresh  and
      McCrae, John  and
      Murray, Kenton  and
      Nakamura, Satoshi  and
      Negri, Matteo  and
      Niehues, Jan  and
      Niu, Xing  and
      Ojha, Atul Kr.  and
      Ortega, John  and
      Papi, Sara  and
      Pol{\'a}k, Peter  and
      Posp{\'\i}{\v{s}}il, Adam  and
      Pecina, Pavel  and
      Salesky, Elizabeth  and
      Sethiya, Nivedita  and
      Sarkar, Balaram  and
      Shi, Jiatong  and
      Sikasote, Claytone  and
      Sperber, Matthias  and
      St{\"u}ker, Sebastian  and
      Sudoh, Katsuhito  and
      Thompson, Brian  and
      Waibel, Alex  and
      Watanabe, Shinji  and
      Wilken, Patrick  and
      Zem{\'a}nek, Petr  and
      Zevallos, Rodolfo},
    editor = "Salesky, Elizabeth  and
      Federico, Marcello  and
      Carpuat, Marine",
    booktitle = "Proceedings of the 21st International Conference on Spoken Language Translation (IWSLT 2024)",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand (in-person and online)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.iwslt-1.1",
    pages = "1--59",
    abstract = "This paper reports on the shared tasks organized by the 21st IWSLT Conference. The shared tasks address 7 scientific challenges in spoken language translation: simultaneous and offline translation, automatic subtitling and dubbing, speech-to-speech translation, dialect and low-resource speech translation, and Indic languages. The shared tasks attracted 17 teams whose submissions are documented in 27 system papers. The growing interest towards spoken language translation is also witnessed by the constantly increasing number of shared task organizers and contributors to the overview paper, almost evenly distributed across industry and academia.",
}
</pre>
<pre>
@inproceedings{moslem-2024-leveraging,
    title = "Leveraging Synthetic Audio Data for End-to-End Low-Resource Speech Translation",
    author = "Moslem, Yasmin",
    editor = "Salesky, Elizabeth  and
      Federico, Marcello  and
      Carpuat, Marine",
    booktitle = "Proceedings of the 21st International Conference on Spoken Language Translation (IWSLT 2024)",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand (in-person and online)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.iwslt-1.31/",
    doi = "10.18653/v1/2024.iwslt-1.31",
    pages = "265--273",
    abstract = "This paper describes our system submission to the International Conference on Spoken Language Translation (IWSLT 2024) for Irish-to-English speech translation. We built end-to-end systems based on Whisper, and employed a number of data augmentation techniques, such as speech back-translation and noise augmentation. We investigate the effect of using synthetic audio data and discuss several methods for enriching signal diversity."
}
</pre>
<pre>
@inproceedings{agrawal-etal-2023-findings,
    title = "{FINDINGS} {OF} {THE} {IWSLT} 2023 {EVALUATION} {CAMPAIGN}",
    author = {Agarwal, Milind  and
      Agrawal, Sweta  and
      Anastasopoulos, Antonios  and
      Bentivogli, Luisa  and
      Bojar, Ond{\v{r}}ej  and
      Borg, Claudia  and
      Carpuat, Marine  and
      Cattoni, Roldano  and
      Cettolo, Mauro  and
      Chen, Mingda  and
      Chen, William  and
      Choukri, Khalid  and
      Chronopoulou, Alexandra  and
      Currey, Anna  and
      Declerck, Thierry  and
      Dong, Qianqian  and
      Duh, Kevin  and
      Est{\`e}ve, Yannick  and
      Federico, Marcello  and
      Gahbiche, Souhir  and
      Haddow, Barry  and
      Hsu, Benjamin  and
      Mon Htut, Phu  and
      Inaguma, Hirofumi  and
      Javorsk{\'y}, D{\'a}vid  and
      Judge, John  and
      Kano, Yasumasa  and
      Ko, Tom  and
      Kumar, Rishu  and
      Li, Pengwei  and
      Ma, Xutai  and
      Mathur, Prashant  and
      Matusov, Evgeny  and
      McNamee, Paul  and
      P. McCrae, John  and
      Murray, Kenton  and
      Nadejde, Maria  and
      Nakamura, Satoshi  and
      Negri, Matteo  and
      Nguyen, Ha  and
      Niehues, Jan  and
      Niu, Xing  and
      Kr. Ojha, Atul  and
      E. Ortega, John  and
      Pal, Proyag  and
      Pino, Juan  and
      van der Plas, Lonneke  and
      Pol{\'a}k, Peter  and
      Rippeth, Elijah  and
      Salesky, Elizabeth  and
      Shi, Jiatong  and
      Sperber, Matthias  and
      St{\"u}ker, Sebastian  and
      Sudoh, Katsuhito  and
      Tang, Yun  and
      Thompson, Brian  and
      Tran, Kevin  and
      Turchi, Marco  and
      Waibel, Alex  and
      Wang, Mingxuan  and
      Watanabe, Shinji  and
      Zevallos, Rodolfo},
    editor = "Salesky, Elizabeth  and
      Federico, Marcello  and
      Carpuat, Marine",
    booktitle = "Proceedings of the 20th International Conference on Spoken Language Translation (IWSLT 2023)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada (in-person and online)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.iwslt-1.1",
    doi = "10.18653/v1/2023.iwslt-1.1",
    pages = "1--61",
    abstract = "This paper reports on the shared tasks organized by the 20th IWSLT Conference. The shared tasks address 9 scientific challenges in spoken language translation: simultaneous and offline translation, automatic subtitling and dubbing, speech-to-speech translation, multilingual, dialect and low-resource speech translation, and formality control. The shared tasks attracted a total of 38 submissions by 31 teams. The growing interest towards spoken language translation is also witnessed by the constantly increasing number of shared task organizers and contributors to the overview paper, almost evenly distributed across industry and academia.",
}
</pre>
<pre>
=== Machine-readable metadata (DO NOT REMOVE!) =====================================================
Data available since: Irish-English Speech Translation Shared Task@IWSLT-2025
License: CC BY-NC-SA 4.0
=======
Includes text/audio: yes
Shared Task Organisers 2025: Ojha, Atul Kr.; Moslem, Yasmin; McCrae, John P.
Contact: atulkumar.ojha@insight-centre.org, shashwatup9k@gmail.com
Contributor/&copy;holder: Insight Research Ireland Centre for Data Analytics, Data Science Institute, University of Galway
=======================================================================================================
</pre>
