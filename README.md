# SignLink: Text-to-Sign Language Translation System with 3D Avatar

## Overview

SignLink is an AI-powered system designed to translate written English text into American Sign Language (ASL) and display the result through a 3D animated avatar. It combines natural language processing, deep learning, and sign-language notation to make written information more accessible to Deaf users.

## How It Works

The system follows a four-stage pipeline:

1. **English-to-Gloss Translation:** Converts English text into ASL gloss using a fine-tuned T5 transformer model.
2. **Gloss-to-HamNoSys Conversion:** Generates phonetic sign notation using neural models and grammar-based validation.
3. **HamNoSys-to-SiGML Conversion:** Converts the notation into SiGML, a structured format for sign-language animation.
4. **3D Avatar Animation:** Uses the JA Signing Avatar to render the generated signs as animations.

## Technologies Used

- **AI & NLP:** Python, T5, Transformer models
- **Computer Vision:** OpenCV, MediaPipe Holistic
- **Deep Learning:** Sequence-to-sequence models, LSTM, attention mechanisms
- **Sign Language Notation:** HamNoSys, SiGML
- **Visualization:** JA Signing Avatar

## Key Features

- Automated English-to-ASL translation pipeline.
- Intermediate gloss representation to account for ASL grammar.
- Neural sign-notation generation with grammar validation.
- Video-based landmark extraction for sign-to-notation research.
- Real-time 3D avatar animation.
- Modular architecture for independent testing and future improvements.

## Results

The project demonstrated successful end-to-end conversion from English text to animated sign output.

- **English-to-Gloss model:** 89.48% accuracy.
- **Avatar rendering:** Successfully generated and displayed signs for tested inputs.
- **Gloss-to-HamNoSys generation:** Learned partial phonological patterns, but exact sequence prediction remained challenging.

The video-based sign-to-notation model was limited by the size and complexity of the annotated dataset. Further improvements require more training data and better phonological representations.

## Future Improvements

- Expand and improve annotated sign-language datasets.
- Improve HamNoSys prediction accuracy.
- Incorporate facial expressions, head movements, and gaze.
- Explore transformer-based models and transfer learning.
- Improve the naturalness and accuracy of avatar animations.

## Project Report

The full project report documents the system architecture, methodology, experiments, results, and limitations.
