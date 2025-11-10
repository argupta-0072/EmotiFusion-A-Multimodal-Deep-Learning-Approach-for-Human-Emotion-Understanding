# 🧠 EmotiFusion: A Deep Learning Model for Emotion Detection from Faces and Text

EmotiFusion is a multimodal deep learning project that detects human emotions by combining facial expression analysis and text-based sentiment understanding. It bridges visual and linguistic modalities using an attention-based fusion architecture, enabling more accurate emotion classification.

## 🚀 Overview

The model integrates two primary components:

Visual Stream: A hybrid CNN network built from ResNet18 and MobileNetV3-Small, pretrained on ImageNet. These extract robust facial features, refined through Channel and Spatial Attention Mechanisms to emphasize the most expressive regions of the face.

Textual Stream: A BERT-based encoder (bert-base-uncased) that transforms dialogues into semantic embeddings representing emotional context in language.

Both 512-dimensional embeddings from the visual and textual streams are fused to produce a joint representation, which is then passed through fully connected layers for final emotion prediction.

## 🎯 Key Features

Multimodal Fusion: Combines vision and text features for holistic emotion understanding.

Attention Mechanisms: Enhances discriminative emotion features at both spatial and channel levels.

Pretrained Backbones: Leverages transfer learning with ResNet, MobileNet, and BERT for better generalization.

8-Class Emotion Recognition: Detects Anger, Contempt, Disgust, Fear, Happy, Neutral, Sad, and Surprise.

Custom Synthetic Dataset: Generates text dialogues for emotion labels, complementing AffectNet’s visual dataset.

## 🧩 Tech Stack

Frameworks: PyTorch, Transformers (Hugging Face), Albumentations

Models: ResNet18, MobileNetV3, BERT-base

Dataset: AffectNet (faces) + Synthetic Emotion Dialogues (text)

Language: Python

## 📈 Results & Goals

EmotiFusion demonstrates the potential of vision-language fusion in emotion AI. Future improvements include real-world video-based emotion recognition and reinforcement-based fine-tuning for conversational agents.
