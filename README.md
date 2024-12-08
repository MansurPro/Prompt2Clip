
# 🎥 **Prompt2Clip**

Prompt2Clip generates high-quality videos from text prompts using YOLOv10 models. Designed for efficiency and flexibility, it fine-tunes object detection models on custom datasets and enables real-time inference for a seamless text-to-video experience.

---

## 🚀 **Key Features**

- **Text-to-Video Conversion**: Converts natural language prompts into video clips.  
- **Custom Dataset Training**: Fine-tunes YOLOv10 models with bird and bee datasets for enhanced detection.  
- **Real-Time Inference**: Supports single-image and streaming video detection.  
- **Cloud-Based Workflow**: Uses Google Colab for GPU-accelerated training and processing.  
- **Customizable Parameters**: Flexible settings for model size, inference steps, and detection thresholds.

---

## 🛠️ **How It Works**

Prompt2Clip combines advanced AI models and custom workflows:
1. **Dataset Integration**: Downloads datasets from Roboflow for custom object detection tasks.
2. **Model Training**: Fine-tunes YOLOv10 on labeled datasets for accurate detection.
3. **Video Generation**: Combines frames generated through detection into cohesive video clips.
4. **Inference Pipelines**: Enables real-time detection on single images or streaming video.

---

## 📂 **Project Structure**

```plaintext
Prompt2Clip/
│
├── datasets/           # Custom datasets for birds and bees
├── models/             # Pre-trained and fine-tuned YOLOv10 models
├── scripts/            # Scripts for training, inference, and video generation
├── examples/           # Example outputs of text-to-video generation
└── README.md           # Project documentation
```

---

## 🖥️ **Usage**

### **1. Clone the Repository**

```bash
git clone https://github.com/MansurPro/Prompt2Clip.git
cd Prompt2Clip
```

### **2. Set Up the Environment**

Run Prompt2Clip in Google Colab for GPU-accelerated operations. Install the required Python packages:

```bash
pip install -r requirements.txt
```

### **3. Train the Model**

```bash
python train.py --dataset datasets/birds --model yolov10m.pt --epochs 10
```

### **4. Run Inference**

```bash
python inference.py --image_path path/to/image.jpg --model_path models/yolov10_best.pt
```

---

## 🎨 **Examples**

| **Prompt**                    | **Generated Video**                |
|--------------------------------|-------------------------------------|
| "A bird flying over a forest"  | [View](examples/bird_forest.mp4)   |
| "A bee hovering near a flower" | [View](examples/bee_flower.mp4)    |

---

## 📊 **Performance**

- **Efficiency**: Fine-tuned for fast and accurate text-to-video generation.  
- **Customizability**: Supports flexible detection thresholds and model configurations.  
- **Scalability**: Leverages GPU resources for high-throughput operations.

---

## 📜 **License**

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## 🙌 **Acknowledgments**

Prompt2Clip builds on the following open-source tools and datasets:
- **YOLOv10** for object detection.
- **Roboflow** for dataset integration.
- **Google Colab** for cloud-based GPU acceleration.

Thank you to the open-source community for enabling innovative solutions like this!
