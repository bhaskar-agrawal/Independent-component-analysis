# Independent-component-analysis
Required Packages: Python(3.0), NumPy, SciPy Toolkit, Matplotlib

In this tutorial we will learn how to solve the Cocktail Party Problem using Independent Component Analysis(ICA). We will first take a look at Principle Component Analysis(PCA). The limitations of PCA will naturally lead to an understanding of what ICA does.
The main project was studied from this link http://home.iitb.ac.in/~shashwat.shukla/ica/
Same python notebook can be run on the google collab  https://colab.research.google.com/notebooks/intro.ipynb#recent=true

It is advised to download the all contents and then putting sounds folder and python notebook under same directory. There might be problem in playing of the sounds apart from VLC media player. 
I am attaching comphrensive tutorial of ICA along with PCA, two algorithms of unsupervised learning. ICA is a signal separation technique which stands on the bases of statistical independence. 
All the recieved sound or any other signals should be non-gaussain. Input signals are passed through some preprocessing steps i.e.. normalisation and whitening. The main idea behind algorithm is central limit theorm. 
For measure of non-gaussianity negentropy is used here, kurtosys is also a measure. 
https://arxiv.org/pdf/1404.2986.pdf
