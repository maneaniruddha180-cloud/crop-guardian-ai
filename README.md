# Crop Guardian: AI-Powered Crop Disease Detection & Advisory Assistant

An AI prototype that helps farmers detect crop diseases from a leaf photo 
and receive grounded, actionable treatment advice — built for the 1M1B 
AI for Sustainability Virtual Internship (IBM SkillsBuild & AICTE).

## Problem
Smallholder farmers often lack timely access to expert diagnosis when 
crops show signs of disease, leading to delayed treatment, yield loss, 
and pesticide overuse from misdiagnosis.

## Solution
Two connected AI components:
1. **Image Classifier** — CNN (MobileNetV2, transfer learning) trained 
   on the PlantVillage dataset predicts the disease class with a 
   confidence score from an uploaded leaf image.
2. **RAG Advisory Assistant** — the predicted disease triggers 
   Retrieval-Augmented Generation: relevant treatment/prevention 
   guidance is retrieved from a curated agricultural knowledge base and 
   passed to an LLM (IBM Granite/IBM BOB), producing a grounded, 
   farmer-friendly recommendation.

## SDG Alignment
- **SDG 2: Zero Hunger** — reduces crop loss from delayed disease response
- **SDG 15: Life on Land** — supports sustainable, lower-pesticide farming

## Tech Stack
- CNN transfer learning (MobileNetV2 / TensorFlow-Keras)
- Retrieval-Augmented Generation (RAG) with vector embeddings
- IBM Granite / IBM BOB for advisory generation
- PlantVillage dataset

## Prototype
See `img1.jpeg` for the app interface mockup and 
`img2.jpeg` for the end-to-end AI pipeline.

## Responsible AI Considerations
- **Fairness:** classifier limitations across regions/lighting flagged; 
  not a replacement for expert diagnosis in ambiguous cases
- **Transparency:** confidence score always shown alongside predictions
- **Ethics:** severe cases explicitly recommend consulting a local 
  agricultural extension officer
- **Privacy:** no farmer personal or location data collected

## Author
Aniruddha Mane ,
Walchand College Of Engineering Sangli
