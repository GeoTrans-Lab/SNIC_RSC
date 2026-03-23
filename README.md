# SNIC_RSC

Research project for Road surface condition classification

## Spatial Data Splitting Part

### Prerequisites
- Python 3.7+

### Required Folder Structure

To run the data splitting notebook (`data_spatial_split.ipynb`), ensure the following structure:

```
.
├── OldData/
│   ├── 0 Undefined/
│   └── 1 Defined/
│       ├── 0 Bare/
│       ├── 1 Centre - Partly/
│       ├── 2 Two Track - Partly/
│       ├── 3 One Track - Partly/
│       └── 4 Fully/
├── NewData/
│   ├── labeled_images.csv
│   ├── 0 Undefined/
│   └── 1 Defined/
│       ├── 0 Bare/
│       ├── 1 Centre - Partly/
│       ├── 2 Two Track - Partly/
│       ├── 3 One Track - Partly/
│       └── 4 Fully/
├── data_spatial_split.ipynb
└── [other project files]
```

**NewData/labeled_images.csv** columns:
- `file_name`, `download_status`, `date_iso`
- `primary_label_id`, `primary_label_name`
- `latitude`, `longitude`, `labeled_by_user_id`

**Supported image formats:** `.jpg`, `.jpeg`, `.png`, `.webp`, `.bmp`, `.tif`, `.tiff`
