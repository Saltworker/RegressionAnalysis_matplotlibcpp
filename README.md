# RegressionAnalysis_matplotlibcpp
Regression analysis tool (class regression) utilizing matplotlibcpp.h to graph the results.
Using .txt files as input, the following can be made:
  - Regression models
     1. Linear (2-part linear is an option)
     2. Exponential
     3. Logarithmic
     4. Power
     5. Second-Degree polynomium [Adjustablue in code]
 - Correlation coefficient(s) hereof [R^2]
 - Graph of regression models
 - Other statistical descriptors [MORE PENDING]
## TO BE DONE:
1. Get scientific values of "inprecise" fixed values
2. Get additional statistical descriptors
## How to import matplotlibcpp.h
This link should do the trick: https://stackoverflow.com/questions/66507618/running-python-matplotlibcpp-in-visual-studio-2019

To sum up the proces of importing matplotlibcpp, here is a checklist:
1. Open command prompt. Enter the following commands:
   - python --version\t (Check if python is installed. Recommended python versions are 3.7 - 3.9)
   - python -m pip install matplotlib
   - python -m pip install numpy
2. Create project (I used visual studio 2022)
3. Download matplotlibcpp.h: https://github.com/lava/matplotlib-cpp/blob/60dcd64c8fd4766e5426f57decfb765422a1d3fe/matplotlibcpp.h#L303
   - SANITY CHECK: Make sure to get rid of  ll. 351-356 inside of matplotlibcpp.h 
4. Move matplotlibcpp.h to project repository. Alternatively include header file via solutions explorer [SHIFT+ALT+L]
5. From the used python repository, include the following under "include Directories":
	- ...\Python37\include
	- ...Python37\Lib\site-packages\numpy\core\include
6. From the used python repository, include the following under "Library Directories":
	- ...\Python37\libs
7. Don't forget to set Solution Configurations to RELEASE
