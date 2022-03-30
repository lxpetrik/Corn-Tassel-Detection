# [![repoheader](https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/ReadMe%20Graphics/repoheader.png)](https://amberbenbow.com)

It is possible to automatically detect corn tassels from high resolution drone (UAV) imagery. The detection of corn tasseling can help farmers pin-point a critical stage in the crop\'s lifecycle in order to provide supplemental irrigation or nutrients. 

Given the today's uncertain climate, it is more important than ever to employ precision agriculture techniques. Between drone flights and reproduceable scripting, it is possible to obtain site specific information to aide that goal.

This GitHub is an exploration of computer vision techniques which can be employed to identify corn tassels.


  ---
 
<p>
  <a href="https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/Code/YOLOX_on_Corn_Tassels_Original_Tutorial.ipynb"><img width="300" align='left' src="https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/ReadMe%20Graphics/transferlearning.png"></a>
</p>
   
### Supervised Transfer Learning

Supervised machine learning is accomplished by providing the algorithm with training data. This training data has been curated to so the algorithm can detect underlying patterns. Transfer learning is when an algorithm has already been trained on vast amounts of data to accomplish a specific task. Transfer learning is especially useful when the amount of training data is sparse as the models can extrapolate fairly well.

For this project, the YOLOX (You Only Look Once X) model was employed for the supervised transfer learning portion. This particular model is trained to detect objects and object classes within images. 

To explore this, please visit the [YOLOX tutorial](https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/Code/YOLOX_on_Corn_Tassels_Original_Tutorial.ipynb) in the Code section of this repo.

 ---

<p>
  <a href="https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/Code/Corn%20Tassel%20Detection%20Techniques%2C%20part%202.ipynb"><img width="300" align='right' src="https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/ReadMe%20Graphics/kmeanscluster.jpg"></a>
</p>
 

### Unsupervised Learning

A downside to supervised machine learning is that creating training data is time intensive. As a result, it is worth exploring the effectiveness of unsupervised machine learning algorithms on the dataset. 

Algorithms such as K-Means and Principal Components Analysis (PCA) do not rely on the time intensive image annotation. Instead, these algorithms are able to detect incredible patterns and group them without the help of humans. 

In this notebook, PCA is used to determine the key features of an image that assist with image segmentation. The image segmentation is accomplished through K-Means. 

To explore this, please visit this [notebook](https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/Code/Corn%20Tassel%20Detection%20Techniques%2C%20part%202.ipynb).

---

<p>
  <a href="https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/Code/Corn%20Tassel%20Detection%20Techniques%2C%20part%201.ipynb"><img width="300" align='left' src="https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/ReadMe%20Graphics/tasselsegmentation.jpg"></a>
</p>

### Other Computer Vision Techniques

Finally, there are additional computer vision techniques which can be employed to explore the dataset. These techniques aid in understanding how best to segment the image. Techniques employed are exploring the RGB and HSV color spaces, histograms and trying different segmentation techniques such as thresholding, watershed segmentation, and random walker segmentation. 

To learn more, please visit this [notebook](https://github.umn.edu/petri142/Corn-Tasseling-Detection/blob/master/Code/Corn%20Tassel%20Detection%20Techniques%2C%20part%201.ipynb).
