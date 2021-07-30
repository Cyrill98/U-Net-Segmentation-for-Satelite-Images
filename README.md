# Semantic Segmentation for-Satelite Images Using U-Net

Kaggle dataset: https://www.kaggle.com/humansintheloop/semantic-segmentation-of-aerial-imagery <br/>
There are 6 categories in this dataset: <br/>
  <li> Building #3C109</li>
  <li> Land #8429F6</li>
  <li> Road #6EC1E4</li>
  <li> Water #E2A929</li>
  <li> Unlabeled #9B9B9B</li>
  
The images comes in various sizes. Hence, we need to preprocess the data so that we can capture all of the images into numpy arrays
    <li>Crop to a size divisible by 256 and extract patches</li>
<br/>
<br/>    
Masks are RGB and information provided as HEX color codeL
  <li> Need to convert HEX to RGB values and then convert RGB labels to integer values and then to          one hot encoded (Multiclass problem)
  Predicted (segmented) images need to converted back into original RGB colors
  Predicted tiles need to be merged into a large image by minimizing blending artefacts( smooth blending)
    
  
