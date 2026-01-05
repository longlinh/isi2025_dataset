# ISI2025 Dataset - Landsat 8 z50

Dataset for the paper: **"Collaborative Self-Training Fuzzy Clustering with Softmax Guidance for Remote Sensing Image Classification"**

## Regions

| Region | Code | Size | Labeled Ratio |
|--------|------|------|---------------|
| Hanoi | hn | 1001×1201 | ~3% |
| Thanh Hoa | th2 | 825×981 | ~7% |
| Ho Chi Minh | hcm2 | 1114×1336 | ~8% |

## Files per Region (7 files each)

Each region folder contains:

| # | File | Description |
|---|------|-------------|
| 1 | `{region}_z50_SR_B2.tif` | Blue band (0.45-0.51 µm) |
| 2 | `{region}_z50_SR_B3.tif` | Green band (0.53-0.59 µm) |
| 3 | `{region}_z50_SR_B4.tif` | Red band (0.64-0.67 µm) |
| 4 | `{region}_z50_SR_B5.tif` | NIR band (0.85-0.88 µm) |
| 5 | `{region}_z50_RGB.tif` | RGB composite |
| 6 | `{region}_z50_labeled_{ratio}pct.tif` | Region-based labeled mask |
| 7 | `{region}_z50_labeled_{ratio}pct.png` | Visualization of labeled regions |

## Label Classes (6 classes)

| Class | Description | Color (PNG) |
|-------|-------------|-------------|
| 0 | Forest | Dark green |
| 1 | Vegetation | Forest green |
| 2 | Water/Wetland | Cyan |
| 3 | Water | Blue |
| 4 | Urban/Built-up | Gray |
| 5 | Agriculture | Bright green |

## Labeling Method

Region-based labeling using circular regions (radius=30 pixels) with different label ratios per site to simulate real-world collaborative learning scenarios.

## Citation

```bibtex
@article{isi2025sefc,
  title={Collaborative Self-Training Fuzzy Clustering with Softmax Guidance},
  author={...},
  journal={...},
  year={2025}
}
```

## License

This dataset is provided for research purposes only.
