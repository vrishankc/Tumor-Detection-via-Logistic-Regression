## Tumor Detection via Logistic Regression
A statistical approach to tumor detection using structured clinical features.

![alt text](https://www.rxdatascience.com/hubfs/Raj%20Files/es1.jpg)

The above image is an example of cancerous (malignant) breast cells next to benign cells. These cells are part of a tumor biopsy where the extracted tissue is sampled with a special needle. The cells are subsequently stained with different dyes to help visualize their shapes, quantity of DNA, etc. These properties provide clues and insight into the rate of cell division (Rapid cell division = Cancerous). 
 ### Optional: Data Feature Descriptions

Our dataset reports 10 different features of the biopsies. Here's what a few of them mean:

1. $Perimeter$: Total distance between points defining the cell's nuclear perimeter.
2. $Radius$: Average distance from the center of the cell's nucleus to its perimeter.
3. $Texture$: The texture of the cell nucleus is measured by finding the variance of the gray scale intensities in the component pixels.
4. $Area$: Nuclear area is measured by counting the number of pixels on the interior of the nucleus and adding one-half of the pixels in the perimeter.

The following image should give a visual to what these cell nucleus features look like: 

![perimeter](https://drive.google.com/uc?export=view&id=1-U43OAojYbMY9gIlpvLHPNr3V2saqqHJ)

5. $Smoothness$: Measures the smoothness of a nuclear contour by measuring the difference between the length of a radial line and the mean length of the lines surrounding it. The image below demonstrates this:

![smoothness](https://drive.google.com/uc?export=view&id=10GokzG7KDKxClJwHPIuIcr3ivvWGRetY)

6. $Concavity$: Measures the severity of concavities or indentations in a cell nucleus. Chords are drawn between non-adjacent snake points and measure the extent to which the actual boundary lies inside each chord. The line in bold in the image below is an example of a chord.

![concavity](https://drive.google.com/uc?export=view&id=1EGdQLX0WAJkM8E598vnKvnMLY2ZVT6Le)

7. $Symmetry$: The major axis (longest chord) through the center is found. Then, the difference between the distance on both sides of the lines that are perpendicular to the major axis is calculated. The image below shows an example of this:

![symmetry](https://drive.google.com/uc?export=view&id=1EMzdkY5TVfA79xInjjeI6b_dYMpCmSSe)


The paper that first detailed these measurements for this dataset can be found here for more information: https://pdfs.semanticscholar.org/1c4a/4db612212a9d3806a848854d20da9ddd0504.pdf 
