# MIAIS_DATASET
**CEA++2022 PAPER**

MIAIS: A Multimedia Recipe Dataset with Ingredient Annotation at Each Instructional Step

## Data collection
MIAIS contains annotation information for 12,000 recipes; each recipe has 9.13 cooking instruction steps on average, each of which is a tuple of a text description and an image.


The text descriptions and images in MIAIS are originated from ***Cookpad***.
We select a subset of Cookpad recipes that 
(1) have at least five cooking steps to ensure sufficient information contained therein 
(2) and contain a text description and an image for every step.

Among 3 million Cookpad recipes, only around 200,000 recipes met our requirement. 
We further randomly selected 12,000 recipes from them. 
We gathered 109,547 pairs of text descriptions and images in total. We note that we will extend our dataset in our future work.

#### The annotation dataset can be downloaded from the zip file in this repository.

## Content in the zip file:

* CookpadAnnotationInfo_index.zip:

    Annotation information about ingredient for each step of each recipe.

    Each file name is named by the ID number we decided from 1 to 12,000 and its original ID in **Cookpad Dataset** can be refered from the file below.
    
    We provide the index of each ingredient in every cooking step we annotated. Since the index is the same as it is in the **Cookpad Dataset**, after you obtain the permission from Cookpad Inc., you can access the original ingredient information by using the index.

* recipeIDInfo.json:

    **The correspondence relationship** between our artificially assigned ID and its original ID.

### The use of the original recipe data should be permitted by Cookpad Inc.



## Reference

If you are interested in our work and want to cite it, please acknowledge the following paper:

@inproceedings{zhang2022miais,
  title={MIAIS: A Multimedia Recipe Dataset with Ingredient Annotation at Each Instructional Step},
  author={Zhang, Yixin and Yamakata, Yoko and Tajima, Keishi},
  booktitle={Proceedings of the 1st International Workshop on Multimedia for Cooking, Eating, and related APPlications},
  pages={49--52},
  year={2022}
}
