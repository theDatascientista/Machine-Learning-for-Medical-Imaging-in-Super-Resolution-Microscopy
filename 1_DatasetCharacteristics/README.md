# Dataset Characteristics


## Dataset Information

### Dataset Source
- **Dataset Link:** https://github.com/Zach-T-Burns/Untrained-PINN-for-SIM
- **Dataset Owner/Contact:** [See link above]

### Data Description
Pixel-based superresolution microscopy images of

  - Clathrin-coated pits (CCP)
  - endoplasmatic reticula (ER)
  - microtubules (MT)
  - F-actin

Fourier Optics of optical imaging systems: 

  - point spread function (PSF)
  - illumination patterns

**Data Structure:**
- 300 samples, for each 1 ground truth image, 1 low resolution image and 25 images obtained with different illumination patterns and PSF.

**Data Composition:**
- ground truth images: 480x480 px;
- low resolution images: 480x480 px;
- input frames with illumination patterns: 120x120 px

**Task Description:**
- The task was to generate a predicted image based on the input frames and the low resolution images.


