# Hieroglyph-Translator
This research-based project focuses on the translation of ancient Egyptian hieroglyphs into English using a deep learning pipeline. The system integrates YOLOv8 for object detection, a custom-trained CNN for classification, and GPT models for generating meaningful English translations.

This project adopted a detection-classification pipeline due to the unavailability of a publicly accessible dataset for ancient hieroglyphs. While a sequence-to-sequence approach for direct sentence generation was initially considered, the lack of comprehensive data with annotations for such tasks made it impractical.

The original dataset of individual hieroglyph images used for this project was sourced from [here](https://github.com/morrisfranken/glyphreader). It is compiled by Morris Franken
Total Images = 4210 
Total Classes = 171
