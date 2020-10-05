# DeepFakeTorch

### Installation

You will need to install cmake first (required for dlib, which is used for face alignment).

```shell
conda create --name torchfakes
activate torchfakes
git clone https://github.com/IanSullivan/DeepFakeTorch.git
cd DeepFakeTorch
pip install requirments.txt
```

### Extract Faces
```shell
python facedetect.py -video_src data_src.mp4 -out_name [directory a or b]
```

---

### Train Model
```shell
python train.py -face_a_dir[location of first faces] -face_b_dir[location of seconds faces] -n_steps 100000
```

---

## Results
Training after 10,000 steps <br>
<img src="images/swapped.gif">
<img src="images/b_to_a.gif">
