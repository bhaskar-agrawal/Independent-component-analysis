# Independent-component-analysis
Required Packages: Python(3.0), NumPy, SciPy Toolkit, Matplotlib

The Cocktail Party Problem(CPP)
So what is the Cocktail Party Problem? Imagine you are at a party where a lot of different conversations are happening in different parts of the room. As a listener in the room, you are receiving sound from all of these conversations at the same time. Given m sources(conversations at the party for example), and some number of sound receivers, separate out the different signals. (We will talk about how many receivers we need later). We need to make some mathematical assumptions and also phrase the problem more formally.
The data
So first of all, our signals here are the sounds coming from different sources. At every (uniformly spaced) discrete interval of time we record m samples, one at each of our m microphones.

Note the implicit assumptions that we have made here:

1) There are as many microphoneses as there are independent conversations(sources) going on in the room.We can say that our system is critically determined(and is not under- or over- determined).
2) Each microphone records a reasonably distinct combination of the independent signals. This simply amounts to not keeping two microphones too close to each other. Due to practical computational limits (see floating point math), it is always best to have easily distinguishable recordings.
One very important thing: We assume that the sound that any receiver records is a linear combination of sounds from the different sources. This is a reasonable assumption to make as pressure adds linearly. Each receiver will receive a different linear combination: If the first receiver is closer to a particular speaker than the second receiver, then the linear weight of this speaker will be proportionately higher for the first receiver.

Courtesy
We further assume that each source is statistically independent with respect to all the other sources. We will look at a mathematical interpretation of statistical independence of two signals later. Within the context of the Cocktail Party parable an intuitive understanding of this assumption follows naturally, as the conversations happening in different parts of the room are independent of each other. Hence, knowing the signal at a particular instant from one source does not allow us to predict the value of the signal from any other source at that instant. They are independent variables. This is the key assumption in Blind Source separation that allows to solve the problem. We are also making one vital assumption about the sources of the signals: that they are non-Gaussian. We will look at what that means and why it matters in the section on Statistical Independence.

This is the basic information what this algorithm is going to do for further details and maths I have attached few links:http://home.iitb.ac.in/~shashwat.shukla/ica/
                                                                                                                         https://arxiv.org/pdf/1404.2986.pdf

Same python notebook can be run on the google collab  https://colab.research.google.com/notebooks/intro.ipynb#recent=true
Steps to run this code:
1.It is advised to download the all contents, by cloning the whole repository.
2.Run this python notebook on jupyter notebook or google collab, in case of google collab first put this full folder on google drive. Then open google collab https://colab.research.google.com/notebooks/intro.ipynb#recent=true, and find this notebook to run. 

Problems that can occur:
1.There might be problem in playing of the sounds apart from VLC media player. 
2.There might be error in running notebook on google collab in that case change the directories.
