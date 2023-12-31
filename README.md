# Personalized-Education-Platform

# Project Overview
This project aims to use machine learning methods to predict if students will answer a specific question correctly based on their previous answers.

# Background
Using an AI model can help gauge student readiness by spotting low-level connections between educational topics. For example, an incorrect answer in one topic may reveal misunderstandings in another topic.

While volunteering as a teacher in Mumbai, I realized the importance of spotting these connections to help students build strong foundations. However, it was challenging to catch every link for every student due to their unique ways of understanding, large class sizes, and even my own unawareness of certain connections.

AI can support teachers in these areas. It could not only pinpoint various knowledge gaps for a student, but also suggest tailored teaching methods for them.

# Technical Implementation
This project uses machine learning models to predict if a student will answer a particular question correctly based on their previous answers. I used the EEDI dataset for training, validation, and testing, which includes responses from 542 students to 1,774 math diagnostic questions. This dataset has three columns: Student ID, Question ID, and whether the answer was correct [1].

I used three different approaches to find the best model: basic autoencoders, optimized autoencoders, and ensemble models. Optimizations included dropout, L2 regularization, momentum, and early stopping with patience, among others.

# Project Results
The best model in this project had a test accuracy of 68.7%. I believe this can be improved further by:

1. Adding more inputs such as age, gender, financial background, and the questions in natural language form.
2. Using bigger datasets. The current dataset is limited for each age because it spans students aged 8 through 17. More data for each age would facilitate comparability, yielding clearer insights.
3. Employing deeper architectures, while ensuring sufficient data and inputs to prevent overfitting.

# Future Applications
Such models can enhance current education systems through:

1. Dynamic updates of questions during a test for comprehensive identification of each individual’s knowledge gaps
2. Integration with LLMs to deliver customized mini-lessons after knowledge gap diagnosis
3. Integration with AI-driven webscrapers to provide appropriate online videos to resolve knowledge gaps
4. Generation of informative educator-facing reports on a class’ most common weaknesses for lesson design

# Citations
[1] Z. Wang, A. Lamb, E. Saveliev, P. Cameron, Y. Zaykov, J. M. Hernández-Lobato, R. E. Turner, R. G. Baraniuk, C. Barton, S. P. Jones, S. Woodhead, and C. Zhang, "Diagnostic questions: The neurips 2020 education challenge," arXiv preprint arXiv:2007.12061, 2020.

[2] I developed this project as part of my CSC 311: Introduction To Machine Learning class. The course staff helped me with functions to facilitate data acquisition and processing, which can be found in the 'utils.py' file.

[3] Dohyun Kim collaborated with me on this project. Dohyun focused on exploring two other approaches for prediction – kNN models and Information Response Theory-based models. The code stored on my GitHub represents only my portion of the work and is separate from Dohyun's contributions.
