# **Howard Craft AI Training Repository**

Welcome to the **Howard Craft AI Training Repository**, the central hub for all training documents, datasets, references, and tools required to build and refine the AI model running inside the **Howard Craft CubeSat-sized Kit** powered by a Raspberry Pi. This repository is designed to be an open-source, collaborative platform for developers, educators, and enthusiasts working to create an intelligent, interactive, and modular robot.

---

## **About Howard Craft**

Howard Craft is a compact, CubeSat-sized robotics platform designed for education, innovation, and entertainment. Equipped with a Raspberry Pi, a Hailo AI chip, and a modular 3D-printed chassis, Howard Craft combines:
- **Conversational AI**: Interact with a friendly, animated face on its screen.
- **Modularity**: Swap components like arms, sensors, and mobility bases.
- **Community-Driven Learning**: Open-source contributions to continuously improve functionality.

This repository supports the AI brain running Howard Craft, ensuring it remains dynamic, engaging, and customizable.

---

## **Repository Structure**

```
HowardCraft-AI/
├── datasets/                    # Datasets for training and fine-tuning AI
│   ├── conversational/          # Dialogue examples for natural language processing
│   ├── object_detection/        # Images and annotations for vision-based tasks
│   ├── decision_making/         # Contextual datasets for robotics behavior
│   └── training_data.json       # Precompiled dataset for initial training
├── training_scripts/            # Scripts for training and fine-tuning models
│   ├── fine_tune_llama3.py      # Fine-tuning the LLaMA3 language model
│   ├── object_recognition.py    # Training for object detection tasks
│   └── model_evaluation.py      # Evaluate and validate trained models
├── pre_trained_models/          # Pre-trained AI models
│   ├── llama3_base_model/       # LLaMA3 base language model
│   ├── audio2face_model/        # Audio2Face animation model for facial expressions
│   └── parakeet_asr_model/      # Parakeet speech-to-text model
├── deployment/                  # Deployment-ready AI models and configurations
│   ├── inference.py             # Code for running AI models locally
│   ├── face_animation/          # Facial animation scripts for the screen
│   └── asr_integration.py       # Speech-to-text integration module
├── docs/                        # Documentation and references
│   ├── setup_guide.md           # Guide to setting up the repository and hardware
│   ├── training_pipeline.md     # Detailed training pipeline walkthrough
│   ├── dataset_guidelines.md    # How to contribute to datasets
│   └── contributing.md          # Guidelines for contributing to the repository
├── examples/                    # Example projects and use cases
│   ├── beginner/                # Simple AI interactions
│   ├── intermediate/            # AI-enabled robotic tasks
│   └── advanced/                # Complex behaviors with modular attachments
├── LICENSE                      # Open-source license details
└── README.md                    # You are here!
```

---

## **Getting Started**

### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/HowardCraft-AI.git
cd HowardCraft-AI
```

### **2. Install Dependencies**
This repository uses Python for training and deployment. Install the required dependencies:
```bash
pip install -r requirements.txt
```

### **3. Set Up Your Hardware**
Ensure you have the following hardware ready:
- **Raspberry Pi 5**
- **Hailo AI Chip**
- **Pi Camera**
- **Screen Display**
- Any optional modular components (e.g., arms, wheels, sensors).

Refer to the [setup guide](docs/setup_guide.md) for detailed instructions.

---

## **Training the AI**

Howard Craft uses a modular training pipeline to fine-tune its AI capabilities. Here's an overview:

### **1. Conversational AI (LLaMA3)**
The conversational model enables Howard Craft to interact with users. Use the `fine_tune_llama3.py` script to train the model on new dialogue datasets:
```bash
python training_scripts/fine_tune_llama3.py --data datasets/conversational/ --epochs 5
```

### **2. Object Detection**
To enable Howard Craft to recognize objects with its camera, train the vision model using the `object_recognition.py` script:
```bash
python training_scripts/object_recognition.py --data datasets/object_detection/ --output pre_trained_models/object_detection_model.pth
```

### **3. Speech-to-Text (Parakeet ASR)**
Enhance Howard Craft's ability to understand speech by updating the ASR model:
```bash
python training_scripts/update_asr_model.py --data datasets/audio_data/
```

---

## **Contributing**

We welcome contributions to improve Howard Craft's AI! Here’s how you can help:
1. **Add New Datasets**:
   - Submit annotated data for conversation, object detection, or decision-making.
   - Follow the guidelines in [dataset_guidelines.md](docs/dataset_guidelines.md).

2. **Improve Scripts**:
   - Optimize training scripts or add new functionality.
   - Submit a pull request with clear documentation.

3. **Share Projects**:
   - Showcase how you’ve customized Howard Craft in the `examples/` folder.

Refer to the [contributing guide](docs/contributing.md) for detailed instructions.

---

## **Community and Support**

Join our community to share ideas, ask questions, and collaborate:
- **GitHub Discussions**: Use the "Discussions" tab for brainstorming and Q&A.
- **Discord**: Join our [Discord server](https://www.craftingtable.com/discord) for real-time collaboration.
- **Email**: Contact us at `support@craftingtable.com`.

---

## **License**

This repository is licensed under the [MIT License](LICENSE), allowing you to freely use, modify, and distribute the code with proper attribution.

---

## **Acknowledgments**

Thank you to all contributors and community members for making Howard Craft possible. Your input drives the innovation behind this project!

---

Happy Building! 🚀
