# Wound Healing Assessment

An AI-based wound healing assessment system that analyzes wound images and tracks wound healing progress over time.

The system is designed to support clinicians by combining computer vision and machine learning with a structured clinical workflow. A wound image can be analyzed to identify the wound region, determine its precise boundary, and extract measurements that can be used to monitor healing over multiple assessments.

## Project Overview

The system follows an AI-powered image analysis pipeline:

**Wound Image → YOLO → U-Net → OpenCV → Measurements → Clinical Review**

- **YOLO** identifies the wound region in the image.
- **U-Net** performs pixel-level segmentation to determine the precise wound boundary.
- **OpenCV** processes the image and segmentation results to calculate wound measurements.
- The resulting assessment can be reviewed by a clinician and compared with previous assessments to track healing progress.

The larger application is designed around a clinical workflow involving **patients, wounds, assessments, AI analysis, clinician review, and healing timelines**.

## Technology Stack

- **Frontend:** React + TypeScript
- **Backend:** Node.js + Express + TypeScript
- **Database:** PostgreSQL
- **Image Storage:** MinIO / S3-compatible object storage
- **ML API:** FastAPI
- **Wound Detection:** YOLO
- **Wound Segmentation:** U-Net
- **Image Processing:** OpenCV
- **Containerization:** Docker

## Goal

The goal of the project is to build a reproducible AI-assisted wound assessment system that can:

- Analyze wound images
- Identify the wound region
- Segment the wound precisely
- Extract wound measurements
- Store assessments over time
- Compare wound progression
- Provide AI results for clinician verification
- Generate a healing timeline and reports

The system is intended as a **clinical decision-support tool**, where AI-generated results are reviewed and verified by a clinician rather than treated as a final diagnosis.
