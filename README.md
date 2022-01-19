# TinderAutoDate

Dating sucks... so why not automate it!

Jokes aside, this was my first implementation of building a convolutional neural network to swipe on tinder for me. Given the obvious ethical and moral dillemas surrounding this, I have never used it in practice, but the edcuational component was fascinating nonetheless. 

The first component of this project involves reverse engineering the tinder API and digging around to build a dataset to train the network on. After finding users near me, and running those images through a quick image standardization script, the network now has data to train on. From there a classification process for user preferences is run to sort into positive and negative folders, which the network can then train itself on. 

The output of this resides in the jupyter notebook which takes in the next user profile, runs it against the trained model, and gives a confidence score of 0-1 on how positive a users taste preferences would rate the profile. If the profile scores higher than a certain confidence threshold, then the bot swipes right and voila, you might just have found true love!
