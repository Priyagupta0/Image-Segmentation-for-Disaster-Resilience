# Image-Segmentation-for-Disaster-Resilience
## Project Overview

This project focuses on developing an image segmentation system to enhance disaster resilience by leveraging machine learning and deep learning techniques. The primary goal is to automatically detect and assess landslide-affected areas using satellite and drone imagery. By processing multispectral, slope, and elevation data, the system provides accurate, pixel-level segmentation to support rapid disaster response and recovery efforts.

- Utilizes the Landslide4Sense dataset for training and evaluation.
- Processes 14-band image patches, including Sentinel-2 multispectral, ALOS PALSAR slope, and DEM data.
- Enables precise mapping of landslide and non-landslide regions.
- Supports scalable analysis for large geographic areas affected by natural disasters.

## Data Description

The Landslide4Sense dataset has three splits, training/validation/test, consisting of 3799, 245, and 800 image patches, respectively. Each image patch is a composite of 14 bands that include:

**Download links:** [training](https://cloud.iarai.ac.at/index.php/s/KrwKngeXN7KjkFm) and [validation](https://cloud.iarai.ac.at/index.php/s/N6TacGsfr5nRNWr).

The _Landslide4Sense_ dataset is structured as follows:
```
├── TrainData/
│   ├── img/
|   |   ├── image_1.h5
|   |   ├── ...
|   |   ├── image_3799.h5
│   ├── mask/
|   |   ├── mask_1.h5
|   |   ├── ...
|   |   ├── mask_3799.h5
├── ValidData/
|   ├── img/
|   |   ├── image_1.h5
|   |   ├── ...
|   |   ├── image_245.h5
├── TestData/
    ├── img/
        ├── image_1.h5
        ├── ...
        ├── image_800.h5
```

Note that the label files (mask files) are only accessible in the training set.
