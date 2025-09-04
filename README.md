# image-captioning-clip-search
Image Captioning with BLIP + CLIP-based Semantic Search on Flickr8k dataset.
🖼️ Image Captioning + CLIP-based Semantic Search
📌 Overview

This project demonstrates a Vision–Language Model (VLM) pipeline that combines image captioning and text-to-image semantic search using modern transformer-based models (BLIP & CLIP).

Image Captioning: Generate natural language captions for images using a pretrained BLIP model.

Image–Text Search: Enable text-based retrieval of relevant images using CLIP embeddings.

✅ This project serves as a stepping stone towards multimodal AI research and can be extended for medical imaging and report generation (e.g., radiology).

🚀 Features

Generate captions for Flickr8k images with BLIP.

Compute CLIP embeddings for both images and captions.

Perform text-to-image retrieval using cosine similarity.

Ready-to-run in Google Colab (no local setup required).

📂 Dataset

Dataset: Flickr8k
.

Contains 8,000 images and 5 captions per image.

In this project, a subset of 1,000 images is used for faster experimentation.

🛠️ Tech Stack

Models: BLIP
, CLIP

Frameworks: PyTorch, HuggingFace Transformers

Platform: Google Colab (GPU-enabled)

📊 Workflow

Generate Captions with BLIP for each image.

Build Image Embeddings using CLIP.

Build Text Embeddings (from generated captions or user queries).

Search Engine: Match text queries with nearest image embeddings.

[ Flickr8k Images ] ──► [ BLIP Captioning ] ──► Captions.csv
       │                           │
       ▼                           ▼
 [ CLIP Image Encoder ]      [ CLIP Text Encoder ]
       │                           │
       └────────────── Shared Embedding Space ───────────────┐
                                                            ▼
                                            [ Text-to-Image Retrieval ]

🎯 Results

Example caption:

Input: 🐶 dog jumping into pool

BLIP Output: “A dog leaps into a swimming pool.”

Example retrieval:

Query: “man riding a horse”

Output: Top-3 most relevant images retrieved from dataset.

📌 How to Run

Open notebook in Google Colab
.

Mount Google Drive & load Flickr8k dataset.

Run cells step by step.

Try text queries in the search function to retrieve matching images.

🔮 Future Work

Extend to medical imaging:

Chest X-ray captioning.

Radiology report retrieval.

Pulmonary nodule temporal reasoning.

Train on larger datasets for better generalization.

👨‍💻 Author

Karno Sarker – Full-stack developer & aspiring AI researcher.
