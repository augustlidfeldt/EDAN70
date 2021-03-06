# Detecting Tissue Damage in Lungs – Alpha Tool
Project in Computer Science - EDAN70

This is the alpha release of a tool for detecting lung tissue damage. The tool is developed to be used in Covid-19 treatment development. 


## Setup
1. Download the [test data](https://github.com/augustlidfeldt/EDAN70/blob/main/Alpha_Release/test) containing histology images from lungs tissue.

2. Download the [model weights](https://github.com/augustlidfeldt/EDAN70/blob/main/Alpha_Release/alpha_weights.h5) and the [labels](https://github.com/augustlidfeldt/EDAN70/blob/main/Alpha_Release/test_newlabels.txt).

3. Open the [Alpha Tool](https://github.com/augustlidfeldt/EDAN70/blob/main/Alpha_Release/Alpha1.ipynb) in Google Colab and upload the test data folder, pretrained model, weights and labels in the side bar menu, placing them in the same directory in the folder /contents/, see image below.

4. Run code and see the results in the classification report output in the console.

5. For testing prediction on a specfic image point out model path in the second cell and run cell.




![File structure](https://github.com/augustlidfeldt/EDAN70/blob/main/Alpha_Release/filestructure.jpg)

## Authors

**August Lidfeldt** - [augustlidfeldt](https://github.com/augustlidfeldt)
**Ludwig Hedlund** - [luuddan](https://github.com/luuddan)

## Acknowledgments

* Thanks to professor Sonja Aits and Dennis Medved for supervising this project.

