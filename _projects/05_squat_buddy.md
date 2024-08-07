---
title: "squat_buddy"
collection: projects
type: "personal project"
permalink: /projects/squat_buddy
---

Python application that gives you biomechanical feedback on your squatting form!

I developed a python app that uses Google's [movenet](https://www.tensorflow.org/hub/tutorials/movenet) to give you feedback on your squatting form.

**Features**
* squat_buddy can project google's movenet model onto a video of you squatting
* Defect detection: squat_buddy has a variety of defects that a it detects when a user is squatting. Some of these features include:
    * Shifting Center of Mass: User sways to one side when they squat
    * Knee-Cave: User's knees wiggle out or cave inwards when squatting
    * Uneven Posterior Ascent: User's rear-area rises at an uneven rate comspared to the upper-back region. This could overload the lower back and increase risk of lower back injury

**In Progress**
* Using a stitched image and CNN to classify squatting form using unsupervised learning
* Using an RNN to characterize positional time-series positional data to classify squats as good or bad

Feel free to checkout my project [here](https://github.com/pranavramachandra1/squat_buddy)!


###### Languages: Python
###### Libraries: OpenCV, Tensorflow, Pandas, Scipy, PyTorch