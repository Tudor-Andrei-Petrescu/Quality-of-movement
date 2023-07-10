# Quality-of-movement

The squat represents a core physical exercise, which has many health benefits, such as the
strengthening of ligaments and bones. Its appeal stems from the fact that it is a simple
exercise, yet effective: targeting a range of muscles, such as the calves, gluteal muscles,
quadriceps and hamstrings. However, incorrect form can cause injuries. Hence it is advis-
able that persons new to performing squats get feedback on their technique to maximise
its benefits and minimise the risk of injuries. Following the COVID-19 pandemic and
with the current cost of living crisis, many people are exercising at home, to save money
on travel and gym fees. However, this removes the possibility of having an expert in the
room when performing physical exercises. As a result, this project represents a first step
in providing automated feedback to people exercising at home.

When assessing the correctness (or quality) of the movement, intuitively one would look at
the posture adopted during the execution, and analyse whether there are any deviations
from what a correct movement should look like. For instance, if a person tucks their chin,
or does not go low enough, these are telling signs that a deviation from the correct posture
has happened. Therefore, the body position adopted by a person (or the 2D coordinates
of the body keypoints if analysing through a sequence of frames) should provide enough
information to be able to determine whether a good form has been adopted during the
squat. Naturally, it follows that the problem can be reduced to a classification problem,
since the mispositions of some body parts are indicative and perhaps enough to separate
a mistake from a correctly executed squat.

This project presents an analysis of the systems which could be used to judge the quality
of the squat exercise. The systems proposed use discriminative Machine Learning models,
such as Support Vector Machines, K-Nearest Neighbours, and Decision Trees, but also
looks at an ensemble, which is the Random Forest. It is concluded that all models with
the exception of the Decision Tree are able to learn to distinguish between the 6 proposed
classes, which are “correct”, “chin tuck”, “leaning forward”, “not low” , “feet close” and
“out knees”.

Lastly, this project proposes and analyses the use of an LSTM model which is tasked
with automatically detecting a squat in a video, without having to manually segment the
video to extract the frames composing the exercise. These results represent something of
a pilot study – being outside the scope of the original project specification and therefore
an extension. Although the system is not tuned to yield excellent results as of yet, it
could provide a baseline for future work in a subsequent project.
The main contributions of this project are:
1. Researched the current achievements within the context of action recognition and quality of movement
2. Used Machine Learning to build a model which is able to separate the types of squats and output the result of a video received as input
3. Looked at the limitations of the proposed dataset, and performed data augmentation to boost the performance of the models
4. Used Deep Learning to create an LSTM which is able to automatically detect the start and end of a squat
