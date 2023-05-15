# PixelSynth: Generating a 3D-Consistent Experience from a Single Image (ICCV 2021)

<img src="docs/teaser.png" align="right" alt="drawing" width="50%">

Chris Rockwell, David F. Fouhey, and Justin Johnson

**[[Project Website](https://crockwell.github.io/pixelsynth/)] [[Paper](https://crockwell.github.io/pixelsynth/data/paper.pdf)] 
[[Supplemental](https://crockwell.github.io/pixelsynth/data/supp.pdf)]**


PixelSynth fuses the complementary strengths of 3D reasoning and autoregressive modeling to create an immersive 3D experience from a single image.

### Installation and Demo
- [Install](docs/INSTALL.md)
- [Demo](docs/DEMO.md)

### Training and Evaluation
- [RealEstate10K](docs/REALESTATE.md)
- [Matterport](docs/MATTERPORT.md)

### Citation
If you use this code for your research, please consider citing:
```
@inProceedings{Rockwell2021,
  author = {Chris Rockwell and David F. Fouhey and Justin Johnson},
  title = {PixelSynth: Generating a 3D-Consistent Experience from a Single Image},
  booktitle = {ICCV},
  year = 2021
}
```

### Special Thanks
Thanks to <a href="https://angelxuanchang.github.io/">Angel Chang</a> and <a href="https://www.3dunderstanding.org/team.html">Angela Dai</a>, 
and Richard Tucker and <a href="https://www.cs.cornell.edu/~snavely/">Noah Snavely</a>,
for allowing us to share frames from their datasets.
Thanks to [Olivia Wiles](https://www.robots.ox.ac.uk/~ow/) and [Ajay Jain](https://www.seas.upenn.edu/~nkolot/) for polished model repositories which were so helpful in this work. 

### Code Organization
```
statue
├── images
│   ├── IMG_2707.jpg
│   ├── IMG_2708.jpg
│   ├── ...
│   └── IMG_2736.jpg
└── images_2
    ├── IMG_2707.png
    ├── IMG_2708.png
    ├── ...
    ├── IMG_2736.png
    └── label
        ├── IMG_2707.png
        ├── IMG_2708.png
        ├── ...
        └── IMG_2736.png
data
demo
docs
evaluation
geometry
models
options
scripts
utils
calc_errors_consistency_homography.py
calc_errors_quality.py
create_nerf_like_circles.py
create_vid.py
demo.py
extract_code.py
extract_pixcnn_orders.py
extract_vqvae_dataset.py
train_dpr.py
train_lmconv.py
train_vqvae.py
```
