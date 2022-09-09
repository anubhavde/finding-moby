#### finding-moby

# **Humpback Whale Identification**

##### Build an algorithm to identify individual whales in images.

After centuries of intense whaling, recovering whale populations still have a hard time adapting to warming oceans and struggle to compete every day with the industrial fishing industry for food.

To aid whale conservation efforts, scientists use photo surveillance systems to monitor ocean activity. They use the shape of whales’ tails and unique markings found in footage to identify what species of whale they’re analyzing and meticulously log whale pod dynamics and movements. For the past 40 years, most of this work has been done manually by individual scientists, leaving a huge trove of data untapped and underutilized.

So my aim is to build an algorithm to identify individual whales in images. For this we’ll need to analyze Happywhale’s database of over 25,000 images, gathered from research institutions and public contributors. This might help to open rich fields of understanding for marine mammal population dynamics around the globe.

Credits for providing this data and problem go to Happywhale. [Happywhale](https://happywhale.com/) is a platform that uses image process algorithms to let anyone to submit their whale photo and have it automatically identified. 

### **Data Description**

The training data contains thousands of images of humpback whale flukes. Individual whales have been identified by researchers and given an Id. The [task](https://www.kaggle.com/competitions/humpback-whale-identification/) is to predict the whale Id of images in the test set. There are only a few examples for each of 3,000+ whale Ids.

### **File descriptions**

- **train.zip** - a folder containing the training images
- **train.csv** - maps the training ```Image``` to the appropriate whale ```Id```. Whales that are not predicted to have a label identified in the training data should be labeled as ```new_whale```.
- **test.zip** - a folder containing the test images to predict the whale ```Id```
- **sample_submission.csv** - a sample submission file in the correct format

Access the dataset(5.95GB) using Kaggle API:
```console
kaggle competitions download -c humpback-whale-identification
```
