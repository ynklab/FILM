# FILM: Fake Illusions for LVLMs

**FILM** is a visual question answering (VQA) task dataset for large vision-language models presented in [COGSCI 2025](https://cognitivesciencesociety.org/cogsci-2025/).

Images in FILM are categorized into genuine and fake illusions, along with corresponding control images.
Genuine illusions present discrepancies between actual and apparent features, whereas fake illusions have the same actual and apparent features even though they look illusory due to the similar geometric configuration. 
Control images are modified versions of illusion images in which the illusion inducing elements are removed to eliminate the illusory effect.

## Data

- **FILM_images/**  
  This folder contains all image files used in the VQA experiments. Subdirectories are organized by image type:
  - `01_genuine_illusion_original/`: Contains genuine illusion images.
  - `02_genuine_illusion_control/`: Contains control images corresponding to genuine illusion images.
  - `03_fake_illusion_original/`: Contains fake illusion images.
  - `04_fake_illusion_control/`: Contains control images corresponding to fake illusion images.

- **FILM_VQA.tsv**  
  A TSV file with VQA annotations. Each row includes:
  - `id`: Unique item ID.
  - `file_name`: Image filename.
  - `question (actual)`, `options (actual)`, `answer (actual)`: Question and answer choices about the image’s actual feature.
  - `question (apparent)`, `options (apparent)`, `answer (apparent)`: Question and answer choices about the image’s apparent feature.
  - `illusion category`: Category of the image’s illusory feature (e.g., `color`, `brightness`, `length`).

## Citation

## Citation
If you use this dataset in any published research, please cite the following manuscript:

- Shinozaki, T., Doi, T., Watahiki, A., Nishida, S., & Yanaka, H. (2025). Do large vision-language models distinguish between the actual and apparent features of illusions? Manuscript accepted for presentation at the 47th Annual Meeting of the Cognitive Science Society. (To appear)

**Note**: The proceedings paper is forthcoming. Please check back for an updated BibTeX entry once it is officially published.

```bibtex
@inproceedings{shinozaki-2025-illusion,
  title     = {Do Large Vision-Language Models Distinguish between the Actual and Apparent Features of Illusions?},
  author    = {Shinozaki, Taiga and Doi, Tomoki and Watahiki, Amane and Nishida, Satoshi and Yanaka, Hitomi},
  booktitle = {To appear in the Proceedings of the 47th Annual Meeting of the Cognitive Science Society},
  year      = {2025},
  note      = {Manuscript accepted for presentation},
}
```

<!--
If you use this dataset in any published research, please cite the following:
- Shinozaki, T., Doi, T., Watahiki, A., Nishida, S., & Yanaka, H. (2025). Do large vision-language models distinguish between the actual and apparent features of illusions? Proceedings of the Annual Meeting of the Cognitive Science Society, 47.

```bibtex
@Inproceedings{shinozaki-2025-illusion,
  title     = "Do Large Vision-Language Models Distinguish between the Actual and Apparent Features of Illusions?",
  author    = "Shinozaki, Taiga and Doi, Tomoki and Watahiki, Amane and Nishida, Satoshi and Yanaka, Hitomi",
  booktitle = "Proceedings of the Annual Meeting of the Cognitive Science Society, 47",
  month     = jul,
  year      = "2025",
  address   = "San Francisco, California",
  publisher = "The Cognitive Science Society",
}
```
-->

## Contact
For questions, please contact snzktig@keio.jp .
## License
- [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)