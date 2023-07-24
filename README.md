# BigBlue-Nearest-Earth-Objects-Classification
Repository for the 3rd project on Supervised ML during my studies in Big Blue Data Academy Data Science &amp; Machine Learning Bootcamp 2023. Engaging with the wonder of space exploration, this repo presents a classification model for NASA's NEOs, distinguishing hazardous ones.

### Dataset used: [NASA - Nearest Earth Objects🚀](https://www.kaggle.com/datasets/sameepvani/nasa-nearest-earth-objects)
### About the Dataset:
#### Context☄️:
Near Earth Objects (NEOs) are comets and asteroids that have been nudged by the gravitational attraction of nearby planets into orbits that allow them to enter the Earth’s neighborhood. Today’s asteroids are the bits and pieces left over from the initial agglomeration of the inner planets that include Mercury, Venus, Earth, and Mars.

There is an infinite number of objects in the outer space. Some of them are closer than we think. Even though we might think that a distance of 70,000 Km can not potentially harm us, at an astronomical scale, this is a minimal distance and can disrupt many natural phenomena. These objects/asteroids can thus prove to be harmful. Hence, it is wise to know what is surrounding us and what can harm us amongst those. Thus, this dataset compiles the list of NASA-certified asteroids that are classified as the nearest Earth object.

#### References🌎:
- [NASA Open API](https://api.nasa.gov/)
- [NEO Earth Close Approaches](https://cneos.jpl.nasa.gov/ca/)

### Analysis & Results📊🕵🏻:
- Dataset was imbalanced so different resampling techniques were used
- The creation of a column named year and extracted by the asteroids' names didn't actually change the model performance
- Pipeline was deployed to evaluate potential pairs for two datasets ( one with the year column and the original), and each result was saved in a dataframe for comparison
- Metrics used for evaluation were focused on balanced accuracy, f1-score macro, and execution time
- The best options were picked and optimized through hyperparameter tuning
- Final decisions were made based on results and focusing mainly on the target which was to minimize the Type II Error (FN predictions)
  
### Conclusion✅🏁:
- Main Goal of the project was succeeded,as the result of the Logistic Regression Model has less than a 1% probability, which means that there is a really small possibility, a NEO to be predicted as non-hazardous while being hazardous!
-  Recall Score for class 1(hazardous) indicates that the model correctly identifies the actual instances of a class characterized as hazardous NEOs
-  In the class of non-hazardous NEOs the model has a great performance for predicting class 0
-  Very good accuracy and time execution
-  On the other hand, the model has a high percentage of False Positive predictions, which means that non-hazardous objects are listed as hazardous, which can have a negative impact in terms of money and budgeting, as we have to observe objects when there is no need! The next step would be to try also minimize the FP%
### Presentation Snapshots📸:
I have included below some snapshots from our presentation.

![Copy of NASA Hazard Classification (1)](https://github.com/DimBakogiannis/BigBlue-Nearest-Earth-Objects-Classification/assets/97474620/036a5199-f8a3-492a-8e5a-a3a039039219)
![Copy of NASA Hazard Classification](https://github.com/DimBakogiannis/BigBlue-Nearest-Earth-Objects-Classification/assets/97474620/8aac93df-50e3-4899-a114-c1b93f8dd443)
![Copy of NASA Hazard Classification (4)](https://github.com/DimBakogiannis/BigBlue-Nearest-Earth-Objects-Classification/assets/97474620/cd9a0080-72a4-4229-add7-8b95f32466c9)
![Copy of NASA Hazard Classification (3)](https://github.com/DimBakogiannis/BigBlue-Nearest-Earth-Objects-Classification/assets/97474620/76160e8b-0e7a-4be5-b64d-1d831fc51dd1)
