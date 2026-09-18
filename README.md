# Computer Vision & YOLO11 Training Guide

A 24-page beginner-to-practitioner study guide covering neural network
fundamentals through to training and deploying a production YOLO11
object detector.

**File:** `CV_and_YOLO11_Training_Guide.pdf`

## Who this is for

Anyone starting out in computer vision who wants one document that goes
from "what is a neural network" all the way to "how do I train and ship
a YOLO11 model responsibly." No prior deep learning background assumed;
basic Python helps for Part 4 onward.

## What's inside

| Part | Title | Covers |
|---|---|---|
| 1 | Foundations — How a Model Actually Learns | Neurons, weights, biases, activation functions, forward pass, loss functions, backpropagation, gradient descent, epochs/batches/learning rate, overfitting & the train/val/test split |
| 2 | Neural Network Architectures: CNN & RNN | Why plain networks fail on images, convolution/kernels/stride/padding/pooling, RNNs and LSTM/GRU, a CNN vs RNN vs Transformer comparison |
| 3 | Object Detection & the YOLO Family | Classification vs. localization vs. detection vs. segmentation, IoU, NMS, mAP, and a version history from YOLOv1 to YOLO11 |
| 4 | Training YOLO11 Step by Step | Installing Ultralytics, YOLO-format dataset layout, the `model.train()` call, a **full parameter reference table** (core settings, optimizer/LR/warmup, loss weights, logging), a **full augmentation parameter table** (`hsv_h`, `mosaic`, `mixup`, `fliplr`, etc.), and how to read `results.csv` / confusion matrices |
| 5 | Training for Production: Do's and Don'ts | Dataset quality & labeling, splitting & data leakage, hyperparameters & reproducibility, export & deployment monitoring — each as a paired Do/Don't box |
| 6 | Study Path & Recommended Videos | Suggested learning order, verified YouTube links (3Blue1Brown's neural network and convolution series, official Ultralytics resources), and a glossary |

## How to use it

- Read Parts 1–3 in order if the underlying math/CV concepts are new —
  each links to a specific video to watch alongside it.
- Jump straight to Part 4 if you already know the theory and just need
  the YOLO11 `train()` argument reference.
- Keep Part 5 open next to your terminal before calling any model
  "production-ready" — it's written as quick-scan Do/Don't checklists.

## Source & accuracy note

Parameter names, types, and defaults in Part 4 are drawn from the
official Ultralytics configuration documentation
(`docs.ultralytics.com/usage/cfg`) at the time this guide was written.
Defaults can shift slightly across `ultralytics` package versions —
cross-check against your installed version's own docs before a
production training run.
