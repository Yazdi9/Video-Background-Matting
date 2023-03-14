# High-Resolution Background Matting

## Paper

[Real-Time High-Resolution Background Matting](https://arxiv.org/abs/2012.07810).  model requires capturing an additional background image and produces state-of-the-art matting results at 4K 30fps and HD 60fps .

## Download

### Model / Weights

* [Download model / weights](https://drive.google.com/drive/folders/1cbetlrKREitIgjnIikG1HdM4x72FtgBh?usp=sharing)

### Video / Image Examples

* [HD videos](https://drive.google.com/drive/folders/1j3BMrRFhFpfzJAe6P2WDtfanoeSCLPiq) (by [Sengupta et al.](https://github.com/senguptaumd/Background-Matting)) (Our model is more robust on HD footage)
* [4K videos and images](https://drive.google.com/drive/folders/16H6Vz3294J-DEzauw06j4IUARRqYGgRD?usp=sharing)


### Datasets

* [Download datasets](https://grail.cs.washington.edu/projects/background-matting-v2/#/datasets)

&nbsp;

## Demo


<div class="center">

 ## Before
 
<https://user-images.githubusercontent.com/33378412/224892651-0974a69c-8b39-4c07-a9a1-45216425b5ae.mp4>


## After
<https://user-images.githubusercontent.com/33378412/224892898-1e24f4be-97f3-4382-8186-c44ee2cc9b86.mp4>


</div>


#### Scripts

We provide several scripts in this repo for you to experiment with our model. More detailed instructions are included in the files.
* `inference_images.py`: Perform matting on a directory of images.
* `inference_video.py`: Perform matting on a video.
* `inference_webcam.py`: An interactive matting demo using your webcam.

#### Notebooks
Additionally, you can try our notebooks in Google Colab for performing matting on images and videos.

* [Image matting (Colab)](https://colab.research.google.com/drive/1cTxFq1YuoJ5QPqaTcnskwlHDolnjBkB9?usp=sharing)
* [Video matting (Colab)](https://colab.research.google.com/drive/1Y9zWfULc8-DDTSsCH-pX6Utw8skiJG5s?usp=sharing)


## Usage / Documentation

You can run our model using **PyTorch**, **TorchScript**, **TensorFlow**, and **ONNX**. For detail about using our model, please check out the [Usage / Documentation](doc/model_usage.md) page.

&nbsp;

## Training

Configure `data_path.pth` to point to your dataset. The original paper uses `train_base.pth` to train only the base model till convergence then use `train_refine.pth` to train the entire network end-to-end. More details are specified in the paper.

&nbsp;


