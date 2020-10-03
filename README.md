

<html>
<div>
<h2>Single Shot Multi-Box Detector: SSD</h2>
  <img alt="er" src="/images/ssd_module.png">
  <br>
  <li><a href='https://arxiv.org/abs/1512.02325'>The paper is here</a></li>
</div>

<div>
<h2>Gradinet-weighted Class Activation Mapping: Grad-CAM</h2>
<p>
Gradient-weighted Class Activation Mapping(Grad-CAM)is an excellent visualization idea for understanding Convolutional Neural Network functions. As more detail explanation of this technique, It uses the gradients of any target concept(say logits for 'dog' or even a caption),flowing into the final convolutional layer to produce a coarse localization map highlighting important regions in an image for predicting the concept. Furthermore, By piling up these localization map onto Guided Backpropagation output, it realizes high level visualization system. There are roughly two algorithm flows. One is the Class Activation Mapping(CAM) and the other one is Guided BackPropagation. CAM is one of the funduamental idea for Grad-CAM.
</p>
<li><a href='https://arxiv.org/abs/1610.02391'>The paper is here</li>
</div>

<div>
  <h2>Directory/File</h2>
  <ul>
    <li>marknet_module/run_marknet.py: モデル実行ファイル(pytorchモデル)</li>
    <li>marknet_module/model/MarkNet.py: MarkNetモデル(pytorch実装)</li>
    <li>marknet_module/utils/create_dataset_csv.py: 学習用画像パスcsvファイルの書き出し</li>
    <li>marknet_module/utils/conduct_gradcam.py: GradCAMモジュール</li>
    <li>marknet_module/utils/data_loader.py: InputPipelinモジュール(pytorch実装)</li>

  </ul>
</div>


<div>
<h2>About SSD Base Code</h2>
  Those codes are derived from the following.<br>
  https://github.com/rykov8/ssd_keras
</div>
<br>
<div>
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)
# A port of [SSD: Single Shot MultiBox Detector](https://github.com/weiliu89/caffe/tree/ssd) to [Keras](https://keras.io) framework.
For more details, please refer to [arXiv paper](http://arxiv.org/abs/1512.02325).
For forward pass for 300x300 model, please, follow `SSD.ipynb` for examples. For training procedure for 300x300 model, please, follow `SSD_training.ipynb` for examples. Moreover, in `testing_utils` folder there is a useful script to test `SSD` on video or on camera input.

Weights are ported from the original models and are available [here](https://mega.nz/#F!7RowVLCL!q3cEVRK9jyOSB9el3SssIA). You need `weights_SSD300.hdf5`, `weights_300x300_old.hdf5` is for the old version of architecture with 3x3 convolution for `pool6`.

This code was tested with `Keras` v1.2.2, `Tensorflow` v1.0.0, `OpenCV` v3.1.0-dev
</div>

</html>
