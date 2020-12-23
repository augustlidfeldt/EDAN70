# Detecting Tissue Damage in Lungs – Final Release
Project in Computer Science - EDAN70

This is the final release of a tool for detecting lung tissue damage. The tool is developed to be used in Covid-19 treatment development. 

## Setup and training
1. Open the [Tissue Damage Classifier](https://github.com/augustlidfeldt/EDAN70/blob/main/Tissue_damage_classifier_final_version/tissue_damage_classifier_final_version.ipynb) in Google Colab. Make sure the histology image data folder is in your Google Drive. Mount your Google Drive with the first cell and change the paths to match your file structure. All subfolders will be created automatically. If you which to change the file placement adapt the code for creating the subfolders. 

2. Run the cell "Images loading and sorting into control, lps_smaller, lps_larger", some sample images will be shown.

3. In the cell "Custom labeling and train test split" choose your severity boundaries and the validation fold you wish to use. Currently three separate validation folds exists, feel free to experiment with these or create your own.

4. Run the cell "Cropping of tiles" to crop the tiles.

5. Run "Data Augmentation" if you wish to apply flipping and rotation to your images. The additional option to augment image brightness is commented out.

6. In the cell "Transfer learning with VGG16" make sure that the TRAIN_DATA_PATH corresponds to the unaugmented/augmented folder depending on which you chose. Also select wheter you want to use Callbacks for storing the progression of precision, recall and F1-score. This will significantly slow down the training process.

7. Run "Transfer learning with VGG16" to train the model. Standard is training for 10 epochs. However the model quickly overtrains, the best model (according to validation accuracy) will be saved as 'best_weights.{epoch}-{val_accuracy}.hdf5'. 

8. Run the subsequent cell to plott precision, recall and F1-score progression during training.

9. Run "Results" to show histogram of predictions and plots of accuracy and loss during the training process.


An incomplete regression model is available a the bottom of the file. The steps to make it work are listed at the top of the last cell.


![File structure](https://github.com/augustlidfeldt/EDAN70/blob/main/Alpha_Release/filestructure.jpg)

## Authors

**August Lidfeldt** - [augustlidfeldt](https://github.com/augustlidfeldt)
**Ludwig Hedlund** - [luuddan](https://github.com/luuddan)

## Acknowledgments

* Thanks to professor Sonja Aits and Dennis Medved for supervising this project.

