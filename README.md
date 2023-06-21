# DryBeanDataset-Classification

Dry Beans Classification Using Machine Learning

Abstract:

 The dry bean is the most widely grown edible legume crop in the world, and it has a diverse genetic makeup. Crop productivity is undoubtedly influenced by seed quality. As a result, seed classification is crucial for marketing as well as production in order to supply the fundamentals of sustainable agricultural systems. Since crop production is in the form of population rather than a single variation, the main goal of this study is to offer a technique for getting homogeneous seed variants. To recognise seven different registered types of dry beans with comparable traits and achieve uniform seed categorization, a computer vision system was created. A high-resolution camera was utilised to capture photos of 13,611 grains from 7 different classified dry bean varieties for the classification model. The MATLAB GUI, or graphical user interface, was used establishing a user-friendly interface. Following segmentation and feature extraction processes on bean pictures obtained using a computer vision system (CVS), a total of 16 features—12 dimension-based and 4 shape-based—were extracted from the grains. Tenfold cross validation was used to develop classification models for Support Vector Machine (SVM), Logistic Regression (LR)and Decision Tree (DT), Random Forest (RF)and performance metrics were compared. For  SVM, LR,  DT and RF, the overall correct classification rates have been found to be 92.61%, 92.50%, 90.32%, and 92.82%, respectively. The Barbunya, Bombay, Cali, Dermason, Horoz, Seker, and Sira bean types were categorised by the SVM classification model, which has the highest accuracy results, with 92.36%, 100.00%, 95.03%, 94.36%, 94.92%, 94.67%, and 86.84%, respectively. With these results, the producers' and consumers' needs for consistent bean types are largely achieved.

Keywords:

Dry bean ,Interquartile range , ADASYN ,Multiclass classification techniques ,Performance measures.

•	Introduction

 Classification of dry beans is of some economic importance. It has become economically significant to classify dry beans. Manual classification requires a lot of labour, etc. More than 13 k samples of dry beans from 7 different species were photographed, and using computer vision techniques, their geometry was evaluated. The set was then examined using a variety of deep learning (also known as artificial neural networks) and machine learning (also known as data science) techniques. Depending on the technique utilised, the overall accuracy was between 87.92 and 93.13%. The UCI machine learning repository has published the dataset used in [1]. In this study, the same dataset is analysed using somewhat different methods. The dimensionality of the data has decreased. Accuracy improvements have been made. Discussion and comparisons have already taken place.


•	Preliminary analysis and visualisation of the dataset

There are 13611 samples in the dataset being examined. A sample consists of 16 geometrical components along with a label that specifies the bean's species. Barbunya, Bombay, Cali, Dermason, Horoz, Seker, and Sira are the different species. Area, perimeter, major axis length, and ConvexArea, Eccentricity, EquivDiameter, Extent, Solidity, Roundness, Compactness, MinorAxisLength, Aspect Ratio, Eccentricity, ShapeFactors 1, 2, 3, and 4 make up the shape factor system. The method by which the features were determined is given in great detail.

The hue of the bean is not disclosed in the geometrical data. It's terrible from a practical standpoint because the colour of many dry bean species varies frequently. On the other hand, if we only want to use the dry bean classification problem as a learning exercise for creating and comparing machine learning models, it is of no significance.

Prediction is based on these beans attributes:

o	Area (A): The area of a bean zone and the number of pixels within its boundaries.

o	Perimeter (P): Bean circumference is defined as the length of its border.

o	Major axis length (L): The distance between the ends of the longest line that can be drawn from a bean.

o	Minor axis length (l): The longest line that can be drawn from the bean while standing perpendicular to the main axis.

o	Aspect ratio (K): Defines the relationship between L and l.

o	Eccentricity (Ec): Eccentricity of the ellipse having the same moments as the region.

o	Convex area (C): Number of pixels in the smallest convex polygon that can contain the area of a bean seed.

o	Equivalent diameter (Ed): The diameter of a circle having the same area as a bean seed area.

o	Extent (Ex): The ratio of the pixels in the bounding box to the bean area.


o	Solidity (S): Also known as convexity. The ratio of the pixels in the convex shell to those found in beans.

o	Roundness (R): Calculated with the following formula: (4piA)/(P^2)

o	Compactness (CO): Measures the roundness of an object: Ed/L

o	ShapeFactor1 (SF1)

o	ShapeFactor2 (SF2)

o	ShapeFactor3 (SF3)

o	ShapeFactor4 (SF4)

o	Class (Seker, Barbunya, Bombay, Cali, Dermosan, Horoz and Sira)



 
