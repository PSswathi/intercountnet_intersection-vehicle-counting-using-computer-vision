# group-emosense-computer-vision


## **Business Problem:**
When organizing a company retreat, a school assembly, or perhaps a community gathering. As the organizer, you're keen to ensure everyone is engaged and enjoying themselves. But how can you gauge the collective mood of the group? That's where this project comes in. The aim is to develop a system capable of analyzing group images to identify the emotions of the individuals within them. By employing deep learning models and algorithms, we aim to identify whether the group is demonstrating happiness, enthusiasm, apprehension, or any other emotional state.

Such a system holds immense potential for various applications. For businesses, it could provide valuable insights into employee satisfaction during team-building events or meetings. In educational settings, it could help educators assess student engagement during lectures or group activities. Even event organizers could leverage this tool to ensure attendees are having a positive experience. Ultimately, by decoding group emotions through visual data, we strive to enhance social dynamics and foster environments favorable to collective well-being and productivity.

## **Existing Solution and Limitations:**

Understanding group emotions from group images is challenging because it involves identifying how each person in the group feels, which can be different for everyone. Traditional methods often treat the whole group as feeling the same way, missing the individual emotions. Also, analyzing group pictures accurately means needing to pick out emotions from both the whole group and each person's face, which can be hard because of different lighting and facial expressions. Plus, emotions can be subtle and vary based on the situation, making it tricky to get it right. Finally, doing this quickly and accurately is important for tasks like managing events or customer interactions.

## **Proposed Solution:**
This project aims to redefine the way we perceive and interpret group emotions by implementing an approach that takes into account the individual emotions within a group. Instead of solely analyzing group images as a whole, our solution involves employing deep learning models to extract emotions of individuals given group images. We strive to create a comprehensive understanding of group emotions that captures the rich diversity of feelings present among group members.

### - Face Detection and Extraction:
- Given an image of a group of people, extract and isolate faces of individual people in the image.
- Use pretrained models such as YOLOv8, YOLOv8 Face, Single-Shot Multibox Detector (SSD), or non-ML algorithmic techniques such as HaarCascade to extract these individual faces.

### - Emotion Classification:
- Once the individual faces have been extracted, identify the emotion of each of the faces in the given image.
Use techniques such as majority voting to identify the emotion of the entire group.
- Use Facial Attribute Analysis from DeepFace library to analyze individual emotions. Feel free to explore other Facial Emotion Recognition models.
Labeling, Validation and Evaluation
- To enable performance validation of the pipeline, we have scrapped about 3000 group images from the internet.
- Label all or a subset of images manually for faces and emotions of each of the faces. You can use a tool such as Label Studio for the same. If you choose to label a subset of images, ensure that there is a diversity in the kind of images you include in your subset.
- Use the labeled images to validate the performance of your solution. Benchmark your solution for latency, as well as against statistical metrics such as Intersection of Union (IoU), Accuracy, Precision, Recall etc.

