<h1>🎵Mood_Based_Music_Recommendation_System</h1>

A Streamlit-based AI project that detects human emotion from an image or webcam feed and recommends music accordingly — giving users a personalized, emotion-aware listening experience.

<h1>❗ Problem with Today’s Music Recommendation Systems</h1>

Most popular music platforms rely heavily on a user's listening history, search behavior, and similar user preferences. Although effective to some extent, these systems suffer from major limitations:
  1. Not Emotion-Aware
  2. Biased Toward Past Behavior
  3. User Has to Do Manual Work
     
<h1>🎯 Our Solution: Mood Based Music Recommendation</h1>
This project makes recommendations based on real-time facial emotion detection using deep learning.
It eliminates the limitations of current systems by understanding how the user feels in the moment.

Our solution uses a combination of <b>Deep Learning, Computer Vision,</b> and <b>Streamlit UI technologies</b>:

<h3>1. Emotion Detection Using Deep Learning</h3>
  -A CNN (Convolutional Neural Network) model is trained on facial expression datasets.
  
  -It recognizes emotions such as Happy, Sad, Angry, Neutral, Fear, Surprise, etc.
  
  -Python libraries used:

   <b>⭐ TensorFlow / Keras</b>

   <b>⭐ OpenCV</b>

   <b>⭐ NumPy</b>

   <b>⭐ Pandas</b>

   <b>⭐ Scikit-learn</b>

<h3>2. Real-Time Image Processing</h3>

  -OpenCV captures webcam frames or processes uploaded images.

  -Faces are detected and preprocessed (resize, grayscale, normalization).

  -Model predicts emotion with a confidence score.

<h3>3. Music Recommendation Engine</h3>

  -Pre-defined playlists mapped to each emotion.

  -Each playlist contains 8 curated YouTube music links.

  -When emotion is detected, the matching playlist is displayed.

<h3>4. Streamlit Web Interface</h3>

  -Provides an interactive and user-friendly UI.

  -Pages include:

   ⭐Home

   ⭐Emotion Detection

   ⭐Music Recommendation

   ⭐Analytics

   ⭐About

<h1>🧠 Model Architecture</h1>

The emotion detection model uses a <b>Convolutional Neural Network (CNN)</b> with the following architecture:

1. Input Layer: 48x48 grayscale images
   
2. Convolutional Layers: 4 blocks with Batch Normalization and Dropout
   
3. Dense Layers: 512 and 256 neurons with regularization
   
4. Output Layer: 7 neurons (one for each emotion)
   
5. Activation: ReLU for hidden layers, Softmax for output
    
<h1>⚙️ How This System Works (Step-by-Step)</h1>

<h3>Step 1: User Input</h3>

The user can either:

1. Upload a photo, or

2. Use webcam for real-time capture

<h3>Step 2: Face & Emotion Analysis</h3>

1. Image is passed to OpenCV

2. Image is preprocessed (resize, grayscale, normalization)

3. CNN model predicts one of the trained emotion categories

4. Recommendations are generated based on detected emotion

<h3>Step 3: Generate Personalized Music Recommendations</h3>

1. Each emotion is linked to its own custom playlist

2. 8 songs are instantly recommended

3. User can click any song → opens directly on YouTube

<h3>Step 4: Show Analytics (Optional)</h3>

1. Emotion confidence score graph

2. Top emotions
   
3. Average confidence score

<h3>Step 5: Seamless User Experience</h3>

The system ensures:

1. Instant detection

2. Relevant recommendations

3. Real-time interactivity

4. Simple, clean UI

<h1>📊Mood Data</h1>

The model is trained on a dataset containing 28,709 images across 7 emotion categories:

1. Happy: 7,215 images

2. Neutral: 4,965 images

3. Sad: 4,830 images

4. Angry: 3,995 images

5. Fear: 4,097 images

6. Surprise: 3,171 images

7. Disgust: 436 images

<h1>📊Music Data</h1>

We use a custom curated playlist dataset, manually defined inside the MusicRecommender class.

For each emotion (Happy, Sad, Angry, Fear, Surprise, Disgust, Neutral), the system stores:

✔️ Genres related to the emotion

✔️ Mood description

✔️ Popular artists associated with that emotional tone

✔️ 8 representative songs (expandable by the user)

✔️ Music attributes like tempo, energy level, and valence

<h1>📈 Performance Metrics</h1>

1. Accuracy: 95%+ on test dataset

2. Processing Time: < 2 seconds per image

3. Model Size: ~50MB

4. Supported Formats: JPG, JPEG, PNG

<h1>💡Creator</h1>

Beerva Joshi , Github : beervajoshi1204

