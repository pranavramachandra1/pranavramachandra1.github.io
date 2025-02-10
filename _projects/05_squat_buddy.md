---
title: "squat_buddy"
collection: projects
type: "personal project"
permalink: /projects/squat_buddy
---

Python application that gives you biomechanical feedback on your squatting form!

I developed a [python app](https://squatbuddy-app-a8afe5b7d5f8.herokuapp.com) that uses Google's [movenet](https://www.tensorflow.org/hub/tutorials/movenet) to give you feedback on your squatting form.

**Learnings**
* **SWE**: Deploying a complex app: this was a 3 step process: developing the model, then deploying a complex environment to host my model, the putting together the web app
* **ML**: Stiching together different models: I went through a variety of ideas, but the most reasonable was using a lightweight 2D model feeding into a lightweight MLP/RFR. 
* **A bunch of the extra stuff in between**: There was a lot to be learned from building, but I learned a lot from the physical deployment stuff, such as building Docker files, and working with a variety of services to develop, build, and host this app (e.g. GCP, AWS S3, EC2, Heroku, etc.)

**Features**
* squat_buddy can project google's movenet model onto a video of you squatting
* Defect detection: I trained a variety of models (random forrest, MLPs: essentially a lightweight model that can run inferences fast!)
* Reasonable-speed video processing: processes videos at a reasonable pace for you to analyze your form during your rest!

**In Progress**
* Making the model faster. Currently, I have deployed my model as a microservice, and use this exposed endpoint to make batch calls a bit more efficient.
* Increasing the accuracy of the model: currently, the model is a multi-class classifier. I have the app working (which is cool), but I am diving deeper on making this model a bit more robust.

Feel free to checkout my project [here](https://squatbuddy-app-a8afe5b7d5f8.herokuapp.com)!


###### Languages: Python, JS
###### Libraries: OpenCV, Tensorflow, Pandas, Scipy, PyTorch, React