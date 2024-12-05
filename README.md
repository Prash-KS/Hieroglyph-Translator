# Hieroglyph-Translator
This research-driven project aims to translate ancient Egyptian hieroglyphs into English using a deep learning pipeline. The system combines YOLOv8 for object detection, a custom-trained CNN for classifying the hieroglyphs, and GPT models to generate meaningful English translations.

The decision to use a detection-classification approach was made because there is no publicly available dataset for hieroglyphs that would allow for a sequence-to-sequence model. Although we initially considered using a sequence-to-sequence method to generate sentences directly, the lack of sufficient annotated data for this type of task made it an impractical solution.

# Dataset
The original dataset of individual hieroglyph images used for this project was sourced from [here](https://github.com/morrisfranken/glyphreader). It is compiled by Morris Franken, each hieroglyph is manually annotated and labelled according the Gardiner Sign List.
Total Images = 4210 
Total Classes = 171

Since the dataset lacked bounding box annotations required for YOLOv8, all images were manually annotated using Roboflow to define regions of interest for detection tasks.

The CNN model showed some promising results and was able to classify the hieroglyphs fairly well. However, the limited amount of data available for such a complex task impacted the performance of the YOLO model. Although YOLO managed to detect the regions of interest, the lack of enough training data resulted in less accurate detections, making it harder for the model to generalize across different images. As a result, the detection quality wasn’t as high as expected.

