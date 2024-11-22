# AdvPatch-1K: An Adversarial T-shirt Dataset for Physical-world Patch Attack Evaluation

## 📌 Dataset Description

**AdvPatch-1K** is specifically tailored for evaluating the robustness of the YOLOv5s object detection model against adversarial attacks in physical environments. By attaching adversarial patches to the surface of T-shirts, this dataset simulates real-world evasion attack scenarios that object detection models may encounter, providing researchers with an abundant collection of test samples and a benchmarking environment.

The physical patches are generated using our novel patch framework, **Diffpatch**, which addresses the challenge faced by current patch generation methods in balancing attack performance and natural appearance. **Diffpatch** is capable of customizing adversarial patches of various shapes and styles based on reference images and masks.

Using **DiffPatch**, we designed **9 adversarial patches** and printed them on T-shirts. We recruited **20 participants** (with ethics approval) to capture images in diverse indoor and outdoor, including laboratories, campus, cafeteria, subway station, and shopping mall. In total, we collected **1,131 images** into **AdvPatch-1K** dataset, including both individual and group (2 to 10+ persons) photos. The dataset is accompanied with detailed annotations of the person and patch locations (bounding boxes). Our dataset provides a valuable resource for advancing defense research against adversarial patch attacks.

## 🎯 Key Features

* **Innovative Approach**: The dataset uniquely combines adversarial attacks with physical environments by applying adversarial patches to T-shirt surfaces, making it an effective tool for testing object detection models' resistance to evasion in real-world settings.
* **Diverse Scenarios**: It includes a variety of shooting conditions, lighting, backgrounds, angles, and movement states.
* **Real-world Context**: Designed to simulate dynamic wear and different environmental conditions, providing valuable insights into how adversarial attacks can affect detection accuracy.

## 📂 Dataset Contents

1. **Image Data**

* Contains images of subjects wearing adversarial T-shirts.
* Varied environments: indoor (laboratories, subway station), outdoor (sunlight, campus, shopping mall).
* Including both individual and group (2 to 10+ persons) photos, stored in different folders.

2. **Annotation Files**

* YOLO-style annotation format for object detection.
* Contains bounding box coordinates (including persons and adversarial patch). The person annotations correspond to the labels folder, and adversarial patch annotations correspond to the adv_labels folder.

3. **File Structure**

```
AdvPatch-1K
    |--1_person
        |--images
            |--0001.jpg
            |--0002.jpg
            ...
        |--labels
            |--0001.txt
            |--0002.txt
            ...
        |--adv_labels
            |--0001.txt
            |--0002.txt
            ...     
    |--2_persons
        ...
    ...
```
## ⚙️ Download
[Download AdvPatch-1K dataset](https://huggingface.co/datasets/xingjunm/AdvPatch-1K)

## 📊 Example Results
1. **Example images from AdvPatch-1K**
![本地图片](example_dataset.jpg)
3. **Adversarial T-shirts**
4. **Some adversarial patches**
5. **Test results on yolov5**

