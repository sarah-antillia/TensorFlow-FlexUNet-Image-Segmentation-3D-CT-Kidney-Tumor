<h2>TensorFlow-FlexUNet-Image-Segmentation-3D-CT-Kidney-Tumor (2026/05/07)</h2>
Sarah T. Arai<br>
Software Laboratory antillia.com<br><br>
This is the first experiment of Image Segmentation for <b>3D-CT-Kidney-Tumor (3 classes)</b> based on 
our <a href="./src/TensorFlowFlexUNet.py">TensorFlowFlexUNet</a>
 (<b>TensorFlow Flexible UNet Image Segmentation Model for Multiclass</b>), and a PNG
 <a href="https://drive.google.com/file/d/1T8EW7ip9XDVstkREqQ3zljYWvzRlWHYn/view?usp=sharing">
3D-CT-Kidney-Tumor-ImageMask-Dataset.zip</a> (<a href="https://creativecommons.org/publicdomain/zero/1.0/">
CC0: Public Domain
</a>), which was derived by us from <br><br>
<a href="https://www.kaggle.com/datasets/fizzazaitoonbsds2022/3d-kidney-tumor-segmentation/data">
<b>3D CT Kidney for Tumor Segmentation
</b>
</a> by Fizza Zaitoon.
<br><br>
<hr>
<b>Actual Image Segmentation for 3D-CT-Kidney-Tumor Images of 512x512 pixels</b><br>
As shown below, the inferred masks predicted by our segmentation model trained by the dataset appear similar to the ground truth masks,
 but they lack precision in certain areas.
<br><br>
<b>class_color_map = {Kidney:blue, Cyst:green, Tumor:red}</b>
<br><br>
<table>
<tr>
<th>Input: image</th>
<th>Mask (ground_truth)</th>
<th>Prediction: inferred_mask</th>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1025_34.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1025_34.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1025_34.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1027_183.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1027_183.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1027_183.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1027_194.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1027_194.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1027_194.png" width="320" height="auto"></td>
</tr>
</table>
<hr>
<br>
<h3>1. Dataset Citation</h3>
The dataset used here was taken from <br><br>
<a href="https://www.kaggle.com/datasets/fizzazaitoonbsds2022/3d-kidney-tumor-segmentation/data">
<b>3D CT Kidney for Tumor Segmentation<br></b>
Annotated 3D kidney CT scans with tumors for research and AI experiments
</a> by Fizza Zaitoon.
<br><br>

The following explanation was taken from the above kaggle web site. 
<br><br>
<b>About Dataset</b><br>
<b>Dataset Description</b><br>
This dataset offers <b>high-quality 3D kidney CT scans</b> with <b>expertly annotated tumors and cysts</b>, 
ideal for AI research in <b>tumor and kidney segmentation</b>.<br>
 Derived from KiTS23, 
it provides full volumetric scans along with precise masks, enabling accurate model development and evaluation.
<br><br>
<b>Highlights</b><br>
<ul>
<li>Total Cases: 489</li>
<li>Composition: 241 Tumor-only, 248 Tumor+Cyst</li>
<li>Annotations: Tumor, Cyst, Kidney, Background</li>
<li>Data Format: .nii.gz 3D CT volumes</li>
<li>Intended Use: Tumor and kidney segmentation</li>
<li>Cons: Only 30/31 cases in this dataset are complete, rest do not have imaging.nii.gz file. (Will try to upload complete soon).</li>
</ul>
<b>Citation</b><br>
<pre>
@misc{heller2023kits21,
  title={The KiTS21 Challenge: Automatic segmentation of kidneys, renal tumors, and renal cysts in corticomedullary-phase CT}, 
  author={Nicholas Heller and Fabian Isensee and Dasha Trofimova and Resha Tejpaul and Zhongchen Zhao and Huai Chen and Lisheng Wang and Alex Golts and Daniel Khapun and Daniel Shats and Yoel Shoshan and Flora Gilboa-Solomon and Yasmeen George and Xi Yang and Jianpeng Zhang and Jing Zhang and Yong Xia and Mengran Wu and Zhiyang Liu and Ed Walczak and Sean McSweeney and Ranveer Vasdev and Chris Hornung and Rafat Solaiman and Jamee Schoephoerster and Bailey Abernathy and David Wu and Safa Abdulkadir and Ben Byun and Justice Spriggs and Griffin Struyk and Alexandra Austin and Ben Simpson and Michael Hagstrom and Sierra Virnig and John French and Nitin Venkatesh and Sarah Chan and Keenan Moore and Anna Jacobsen and Susan Austin and Mark Austin, Subodh Regmi, Nikolaos Papanikolopoulos, Christopher Weight},
  year={2023},
  eprint={2307.01984},
  archivePrefix={arXiv},
  primaryClass={cs.CV}
}

</pre>
<br>
<b>License</b><br>
<a href="https://creativecommons.org/publicdomain/zero/1.0/">
CC0: Public Domain
</a>
<br>
<br>
<h3>
<a id="2">
2 3D-CT-Kidney-Tumor ImageMask Dataset
</a>
</h3>
 If you would like to train this 3D-CT-Kidney-Tumor Segmentation model by yourself,
 please download the dataset from the google drive  
 <a href="https://drive.google.com/file/d/1T8EW7ip9XDVstkREqQ3zljYWvzRlWHYn/view?usp=sharing">
3D-CT-Kidney-Tumor-ImageMask-Dataset.zip</a> (<a href="https://interoperable-europe.ec.europa.eu/licence/creative-commons-attribution-40-international-cc-40">
CC BY 4.0
</a>)
, expand the downloaded ImageMaskDataset and put it under <b>./dataset</b> folder to be
<br>
<pre>
./dataset
└─3D-CT-Kidney-Tumor
    ├─test
    │   ├─images
    │   └─masks
    ├─train
    │   ├─images
    │   └─masks
    └─valid
        ├─images
        └─masks
</pre>
<br>
<b>3D-CT-Kidney-Tumor Statistics</b><br>
<img src ="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/3D-CT-Kidney-Tumor_Statistics.png" width="512" height="auto"><br>
<br>
As shown above, the number of images of train and valid datasets is large enough to use for the
 training set of our segmentation model.
<br>
<br>
We used a simple Python script to generate our 
PNG dataset with colorized masks from the pairs of <b>"*imaging.nii.gz"</b> and
<b>"*segmentation.nii.gz"</b> of 3D-CT-Kidney-Tumor.
For simplicity, we excluded all empty black masks and their corresponding images,
which were irrelevant to train our segmentation model.<br><br>
.
<b>Train sample images</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/train_images_sample.png" width="1024" height="auto">
<br>
<b>Train sample masks</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/train_masks_sample.png" width="1024" height="auto">
<br>

<h3>
3 Train TensorFlowFlexUNet Model
</h3>
 We trained 3D-CT-Kidney-Tumor TensorFlowFlexUNet Model by using the 
<a href="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/train_eval_infer.config"> <b>train_eval_infer.config</b></a> file. <br>
Please move to ./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor and run the following bat file.<br>
<pre>
>1.train.bat
</pre>
, which simply runs the following command.<br>
<pre>
>python ../../../src/TensorFlowFlexUNetTrainer.py ./train_eval_infer.config
</pre>
<hr>

<b>Model parameters</b><br>
Defined a small <b>base_filters=16 </b> and large <b>base_kernels=(11,11)</b> for the first Conv Layer of Encoder Block of 
<a href="./src/TensorFlowFlexUNet.py">TensorFlowFlexUNet.py</a> 
and a large <b>num_layers=8</b> (including a bridge between Encoder and Decoder Blocks).
<pre>
[model]
;You may specify your own UNet class derived from our TensorFlowFlexModel
model         = TensorFlowFlexUNet"
image_width    = 512
image_height   = 512
image_channels = 3
input_normalize = True
normalization  = False
num_classes    = 4
base_filters   = 16
base_kernels   = (11,11)
num_layers     = 8
dropout_rate   = 0.04
dilation       = (1,1)
</pre>
<b>Learning rate</b><br>
Defined a small learning rate.  
<pre>
[model]
learning_rate  = 0.00007
</pre>
<b>Loss and metrics functions</b><br>
Specified "categorical_crossentropy" and <a href="./src/dice_coef_multiclass.py">"dice_coef_multiclass"</a>.<br>
<pre>
[model]
loss           = "categorical_crossentropy"
metrics        = ["dice_coef_multiclass"]
</pre>
<b>Dataset class</b><br>
Specifed <a href="./src/ImageCategorizedMaskDataset.py">ImageCategorizedMaskDataset</a> class.<br>
<pre>
[dataset]
class_name    = "ImageCategorizedMaskDataset"
</pre>
<br>
<b>Learning rate reducer callback</b><br>
Enabled learing_rate_reducer callback, and a small reducer_patience.
<pre> 
[train]
learning_rate_reducer = True
reducer_factor     = 0.4
reducer_patience   = 4
</pre>
<b>Early stopping callback</b><br>
Enabled early stopping callback with patience parameter.
<pre>
[train]
patience      = 10
</pre>
<b>RGB Color map</b><br>
Specifed rgb color map dict for 3D-CT-Kidney-Tumor 1+3 classes.<br>
<pre>
[mask]
mask_datatyoe    = "categorized"
mask_file_format = ".png"
;3D-CT-Kidney-Tumorrgb color map dict for 1+3 classes.
;                      Kidney:blue,   Cyst:green,  Tumor:red
rgb_map = {(0,0,0):0, (0,0,255):1, (0,255,0):2, (255,0,0):3 }
</pre>
<b>Epoch change inference callback</b><br>
Enabled <a href="./src/EpochChangeInferencer.py">epoch_change_infer callback</a></b>.<br>
<pre>
[train]
epoch_change_infer       = True
epoch_change_infer_dir   =  "./epoch_change_infer"
num_infer_images         = 6
</pre>
By using this callback, on every epoch_change, the inference procedure can be called
 for 6 images in <b>mini_test</b> folder. This will help you confirm how the predicted mask changes 
 at each epoch during your training process.<br> 
<br> 
<!--
As shown below, early in the model training, the predicted masks from our UNet segmentation model showed 
discouraging results.
 However, as training progressed through the epochs, the predictions gradually improved. 
 <br> 
-->
<br>
<b>Epoch_change_inference output at starting (epoch 1,2,3)</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/epoch_change_infer_at_start.png" width="1024" height="auto"><br>
<br>
<b>Epoch_change_inference output at middlepoint (epoch 16,17,18)</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/epoch_change_infer_at_middle.png" width="1024" height="auto"><br>
<br>

<b>Epoch_change_inference output at ending (epoch 32,33,34)</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/epoch_change_infer_at_end.png" width="1024" height="auto"><br>
<br>

In this experiment, the training process was stopped at epoch 46 by EarlyStopping callback.<br><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/train_console_output_at_epoch34.png" width="1024" height="auto"><br>
<br>

<a href="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/eval/train_metrics.csv">train_metrics.csv</a><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/eval/train_metrics.png" width="520" height="auto"><br>

<br>
<a href="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/eval/train_losses.csv">train_losses.csv</a><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/eval/train_losses.png" width="520" height="auto"><br>
<br>
<h3>
4 Evaluation
</h3>
Please move to <b>./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor</b> folder,<br>
and run the following bat file to evaluate TensorFlowUNet model for 3D-CT-Kidney-Tumor.<br>
<pre>
./2.evaluate.bat
</pre>
This bat file simply runs the following command.
<pre>
python ../../../src/TensorFlowFlexUNetEvaluator.py ./train_eval_infer_aug.config
</pre>

Evaluation console output:<br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/evaluate_console_output_at_epoch34.png" width="1024" height="auto">
<br><br>Image-Segmentation-3D-CT-Kidney-Tumor

<a href="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/evaluation.csv">evaluation.csv</a><br>
The loss (categorical_crossentropy) to this <b>3D-CT-Kidney-Tumor/test</b> was not low and dice_coef_multiclass not high as shown below.
<br>
<pre>
categorical_crossentropy,0.0031
dice_coef_multiclass,0.9983
</pre>
<br>
<h3>
5 Inference
</h3>
Please move to a <b>./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor</b> folder<br>
,and run the following bat file to infer segmentation regions for images by the Trained-TensorFlowUNet model for 3D-CT-Kidney-Tumor.<br>
<pre>
./3.infer.bat
</pre>
This simply runs the following command.
<pre>
python ../../../src/TensorFlowFlexUNetInferencer.py ./train_eval_infer_aug.config
</pre>
<hr>
<b>mini_test_images</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/mini_test_images.png" width="1024" height="auto"><br>
<b>mini_test_mask(ground_truth)</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/mini_test_masks.png" width="1024" height="auto"><br>
<hr>
<b>Inferred test masks</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/asset/mini_test_output.png" width="1024" height="auto"><br>
<br>
<hr>
<b>Enlarged images and masks of 3D-CT-Kidney-Tumor Images</b><br>
As shown below, the inferred masks predicted by our segmentation model trained by the dataset appear similar to the ground truth masks,
 but they lack precision in certain areas.
<br><br>
<b>class_color_map = {Kidney:blue, Cyst:green, Tumor:red}</b>
<br><br>
<table>
<tr>
<th>Image</th>
<th>Mask (ground_truth)</th>
<th>Inferred-mask</th>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1023_353.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1023_353.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1023_353.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1024_73.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1024_73.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1024_73.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1026_60.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1026_60.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1026_60.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1027_183.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1027_183.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1027_183.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1027_193.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1027_193.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1027_193.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/images/1027_197.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test/masks/1027_197.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_output/1027_197.png" width="320" height="auto"></td>
</tr>
</table>
<hr>
<br>
<br>
<h3>
6 3D Volume Segmentation
</h3>
Please move <b>./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor</b> folder, and run the following bat file to infer images segmentation for 2D slices of 3D volume NIfTI files
 by the Trained-TensorFlowFlexUNet model for 3D-CT-Kidney-Tumor.<br>
<pre>
>./5.infer3d.bat
</pre>
This simply runs the following command.
<pre>
>python ../../../src/TensorFlowFlexUNet3DInferencer.py ./train_eval_infer.config
</pre>

<b>infer3d section </b> in <a href="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/train_eval_infer.config">
train_eval_infer.config
<a></b>
<pre>
[infer3d] 
;Specify an images_dir which contains NIfTI files
images_dir    = "./mini_test_3d/images/"
output_dir    = "./mini_test_3d_output/"
slice_shape_order = "dhw"
slice_normalize = False
slice_resize   = (512,512)
slice_rotation = None
mask_overlay  = True
</pre>
<hr>
<b>Acutual Image Segmentation for 2D Slices of a 3D-CT-Kidney-Tumor NIfTI</b><br>
Some Slices, Inferred Masks and Mask overlays for a 3D volume <b>case_00016_imaging.nii.gz</b> file.<br>
<br>
<b>class_color_map = {Kidney:blue, Cyst:green, Tumor:red}</b>
<br>
<table>
<tr>
<th>Input: Slice</th>
<th>Prediction: Inferred mask</th>
<th>Mask Overlay</th>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/slices/10048.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/masks/10048.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/overlays/10048.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/slices/10050.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/masks/10050.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/overlays/10050.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/slices/10057.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/masks/10057.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/overlays/10057.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/slices/10061.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/masks/10061.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/overlays/10061.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/slices/10065.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/masks/10065.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/overlays/10065.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/slices/10070.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/masks/10070.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/mini_test_3d_output/case_00016_imaging.nii.gz/overlays/10070.png" width="320" height="auto"></td>

</tr>
</table>
<hr>
<br>
<br>
<h3>
7 MaskOverlay Video of 3D Volume Segmentation
</h3>
Please move to <b>./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor</b> folder, and run the following bat file 
to generate <b>overlays.mp4</b> or <b>overlay.gif</b> for MaskOverlays of 3D Volume Segmentation. <br>
<pre>
>./6.video3d.bat
</pre>
This simply runs the following command.
<pre>
>python ../../../src/MaskOverlayVideoGenerator.py ./train_eval_infer.config
</pre>
<br>

<b>infer3d section </b> in <a href="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/train_eval_infer.config">
train_eval_infer.config
<a></b>

<pre>
[infer3d] 
mask_overlay  = True
;Specify ".mp4" or ".gif".
;video_fileformat  = ".mp4"
video_fileformat  = ".gif"
</pre>
<br>
<b>overlays.gif</b><br>
<img src="./projects/TensorFlowFlexUNet/3D-CT-Kidney-Tumor/video_3d/overlays.gif">
<br>
<br>
<h3>
References
</h3>
<b>1. TensorFlow-FlexUNet-Image-Segmentation-KiTS19-Kidney-Tumor</b><br>
Toshiyuki Arai<br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-KiTS19-Kidney-Tumor">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-KiTS19-Kidney-Tumor</a>
<br><br>
<b>2. TensorFlow-FlexUNet-Image-Segmentation-Model</b><br>
Toshiyuki Arai<br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Model">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Model</a>
<br><br>

