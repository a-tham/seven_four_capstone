### Seven/Four: Music Genre Prediction and Audio Sample Recommendation

Please refer to the PDF slides (seven_four_capstone.pdf) for further details.

This is a project that helps musicians seeking to find audio samples via a song genre prediction.

Please check requirements.txt for the running of the main Jupyter notebook (seven_four.ipynb).

Please check requirements_working_file.txt for the running of the full project Jupyter notebook (seven_four_working_file.ipynb)

### Why Seven/Four?

Seven/Four (stylised as 7/4) is an uncommon and unique time signature notation that indicates having 7 beats in a bar, instead of the common 4/4 time signature.

### What does Seven/Four do?

Seven/Four is a music genre prediction & sample recommendation system.
 
Its aim is to provide musicians an all-in-one method to obtain royalty-free audio samples related to the genre of a track selected. The samples can then be used in a digital audio workstation.

Seven/Four checks what a user wants to listen to via the artist input, and then it will proceed to ask for album and track before hitting Spotify's API to
obtain the 30s preview URL.

The library module, Librosa, proceeds to convert these into Mel-spectrograms before running it through the Conv1D neural network.

The neural network currently runs 3 convolution layers and a dense layer to predict across 7 genres.

The genre will recommend 5 audio samples derived from Freesound's API, which is ready for downloading and usage.

I intend to deploy this project for usage to test out its function in public.

### The Long Read

If you've read this far and have gotten curious as to how this all came about, here's a wall of text discussing it all.

You've been warned!

Seven/Four is a capstone project done during General Assembly (Singapore) by yours truly, Alvin Tham.
It originally started out as an exploratory experiment with the knowledge that I was gaining daily, as well as my love for music, through the gruelling bootcamp. The experiment started to flesh itself out and I realised eventually that this project of labour was something that I really wanted to work on and present as my capstone project.

At the very start, the only piece I had was being able to hit Spotify's API as we had just covered APIs in class.
This initial piece was what sparked everything off, as I started to check out Spotify's API functions, and then eventually use
Last.FM's API as well for practice. At this point in time, a subtle notion started forming in my mind: Predicting music genres.

As I was a keen follower of Google's Tensorflow and it so happened that Tensorflow 2.0 Beta was released, I thought to myself, 
hey, here's an opportunity to try and learn it whilst doing something that was in my mind. Considering that Tensorflow 2.0
Beta was easier to learn with Keras being adopted as its high level API, I decided to put everything I had within me to proceed with music genre prediction. Carpe diem!

So what transpired after? Well, basically:

- Read a lot of research papers
- Read a lot on audio signal processing
- Researched on the neural network architectures used in aforementioned research papers
- Decided to obtain my own samples instead of using datasets from Kaggle, by way of Spotify
- Decided to create and train my own neural network instead of copying others
- Many long nights curating and obtaining Spotify playlists to train the model for 7 genres
- Many long nights iterating through various audio features and extractions
- Many long nights training and adjusting my neural network
- Decided to deploy the model, which meant learning back-end and front-end development
- Many long nights putting together the back and front end (not a web developer here, everything's new to me and learning!)

Admittedly, it won't be that great looking of a website, but it's enough for now to serve its purpose.

This project will continue to be developed and worked on.