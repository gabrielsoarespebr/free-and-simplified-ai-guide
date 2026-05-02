# The Big Picture of Technology

|         | [Artificial Intelligence (AI)](#inside-artificial-intelligence-ai) | Software Development                     | Cybersecurity                                              | IT Support                                | Infrastructure / DevOps | Data & Analytics                       | Networking                 | Cloud Computing                              | Embedded Systems / IoT |
| ------- | ------------------------------------------------------------------ | ---------------------------------------- | ---------------------------------------------------------- | ----------------------------------------- | ----------------------- | -------------------------------------- | -------------------------- | -------------------------------------------- | ---------------------- |
| Goal    | Make machines perform tasks that normally require human abilities  | Create apps, websites and systems        | Protect data and systems from hackers                      | Keep devices and systems working properly |                         | Turn data into useful insights         | Connect devices            | Store data and run systems over the internet |                        |
| Example | ChatGPT doing your homework                                        | Netflix for smartphones, browsers and PC | Blue Team detecting suspicious login attempts in a website | Installing operating systems in a PC      |                         | Spotify showing your most played songs | You enabling Wi-Fi at home | Google Drive storing your files              |                        |

---

# Inside Artificial Intelligence (AI)

|         | [Machine Learning (ML)](#inside-machine-learning-ml) | Computer Vision                | Natural Language Processing (NLP) | Robotics                |
| ------- | ---------------------------------------------------- | ------------------------------ | --------------------------------- | ----------------------- |
| Goal    | Human ability: Learning                              | Human ability: Vision          | Human ability: Communication      | Human ability: Movement |
| Example | ChatGPT doing your homework                          | Face recognition on your phone | Google Maps voice navigation      | Robot vacuum cleaners   |

---

# Inside Machine Learning (ML)

<div align="center">
  <a href="https://assets.qlik.com/image/upload/w_1600/q_auto/qlik/glossary/augmented-analytics/seo-machine-learning-vs-ai-how-ml-ai-work-together_hdgcbz.png">
    <img src="https://assets.qlik.com/image/upload/w_1600/q_auto/qlik/glossary/augmented-analytics/seo-machine-learning-vs-ai-how-ml-ai-work-together_hdgcbz.png" width="600" alt="Hierarchical diagram showing Deep Learning inside Neural Nets inside Machine Learning inside Artificial Intelligence"/>
  </a>
  <br/>
  <em>Image source: Qlik</em>
</div>

If Machine Learning (ML) focuses on learning, there is a subset of ML called [Deep Learning](#inside-deep-learning), which uses neural networks inspired by the human brain to solve the complex problems.

---

# Inside Deep Learning

|         | Generative AI                                    | Discriminative AI           |
| ------- | ------------------------------------------------ | --------------------------- |
| Goal    | Create new content                               | Classify or predict content |
| Example | Gemini using Nano Banana to generate a dog image | Spam filter                 |

---
# What is Machine Learning (ML)?

- Machine Learning (ML): the process of training a [model](#what-is-a-model) to perform a task using data.

> [!NOTE]
ML isn't a silver bullet, don't try to solve every problem with ML.
In many cases, it can be overkill, like using a sledgehammer to crack a nut.
First, try to imagine a solution without ML (heuristic solution), then evaluate whether an ML approach actually adds value to your solution in terms of quality, cost, time savings, and performance.

## Types of ML Systems

- According to the task: [Generative or Discriminative](#inside-deep-learning)
- According to the learning type: Supervised learning, Unsupervised learning or Reinforcement learning

|              | Supervised learning                                                                      | Unsupervised learning                                                                                                                                                                    | Reinforcement learning                                                                                                                      |
| ------------ | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Meaning      | Training a model using features and their corresponding labels                           | Training a model using features without labels                                                                                                                                           | Training an agent through interaction with an environment using rewards and penalties                                                       |
| Source       | Labeled data (features + labels)                                                         | Unlabeled data (features only)                                                                                                                                                           | Rewards and penalties (trial and error)                                                                                                     |
| Jargons      | Feature (input), Label (target/output)                                                   | Feature (input), Pattern                                                                                                                                                                 | Policy                                                                                                                                      |
| Analogy      | Studying for an exam using answered exams. Questions are features and answers are labels | Organizing a box of mixed objects by similarity without knowing the categories beforehand. Features are object characteristics and pattern are the groups based on these characteristics | Giving a dog a treat after it obeys the "sit" command. Policy is the rule the dog learns: sitting leads to a reward, while jumping does not |
| Common cases | [Regression and classification](#supervised-learning-common-cases)                       |                                                                                                                                                                                          |                                                                                                                                             |

<div align="center">
  <a href="https://assets.qlik.com/image/upload/w_1600/q_auto/qlik/glossary/augmented-analytics/seo-machine-learning-vs-ai-how-ml-ai-work-together_hdgcbz.png">
    <img src="https://developers.google.com/static/machine-learning/intro-to-ml/images/labeled_example.png" width="600" alt="Features and label in a weather model that predicts rainfall"/>
  </a>
  <br/>
  <p>Features and label in a weather model that predicts rainfall</p>
  <em>Image source: Google Developers</em>
</div>

---

### Supervised learning common cases

Regression and classification are the two most common supervised learning cases:
- Regression: predict a numeric value. (e.g., house price)

<div align="center">
  <a href="https://developers.google.com/machine-learning/problem-framing/ml-framing">
    <img src="https://developers.google.com/static/machine-learning/problem-framing/images/regression-model.png" width="300" alt="A regression model making a numeric prediction"/>
  </a>
  <br/>
  <em>Image source: Google Developers</em>
  <p>A regression model making a numeric prediction</p>
</div>


- Classification: predict which category an input belongs to by estimating probabilities.
  - Binary classification: two possible classes (e.g., whether it will rain or not).
  - Multiclass classification: multiple classes (e.g., classifying an animal in an image as a cat, dog, or bird).

<div align="center">
  <a href="https://developers.google.com/machine-learning/problem-framing/ml-framing">
    <img src="https://developers.google.com/static/machine-learning/problem-framing/images/classification-model.png" width="300" alt="A regression model making a numeric prediction"/>
  </a>
  <br/>
  <em>Image source: Google Developers</em>
  <p>A classification model making predictions</p>
</div>

---

# What is a model?

- Model: Mathematical function that maps inputs to outputs with parameters learned from data.

## Types of model

|                 | Untrained model                                                                                                                                                                            | Pre-trained model                                                                                                                                                                                                                                                          | Trained model                                                                                                                                                                                                                                                     |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Parameters      | Random parameters                                                                                                                                                                          | Parameters learned from general data                                                                                                                                                                                                                                       | Parameters learned from specific data                                                                                                                                                                                                                             |
| Patterns        | No patterns                                                                                                                                                                                | General patterns                                                                                                                                                                                                                                                           | Specific pattern                                                                                                                                                                                                                                                  |
| Didatic example | Considering the size of a house as x, predict the price of a house in your neighborhood with y = 2x + 10. Why 2 and 10? No reason, the model is useless because the parameters are random! | Considering the size of a house as x, predict the price of a house in your neighborhood with y = 3000x + 50000. Why 3000 and 50000? Because these are the parameters for an average house around the world, so the model can be reused if fine-tuned to your neighborhood. | Considering the size of a house as x, predict the price of a house in your neighborhood with y = 4000x + 20000. Why 4000 and 20000? Because these are exactly the parameters for a average house in your neighborhood, which makes the model accurate/fine-tuned. |

---

# Other:
- Main sources:
  - Courses:
    - [Introduction to Generative AI](https://www.skills.google/paths/118/course_templates/536) (By Google Cloud Skills Boost)
    - [Introduction to Machine Learning](https://developers.google.com/machine-learning/intro-to-ml) (By Google for Developers)
  - Books:
    - Hands-On Machine Learning with Scikit-Learn, Keras, and Tensorflow: Concepts, Tools, and Techniques to Build Intelligent Systems (By Aurélien Géron)

- Author info
  - LinkedIn: [gabrielsoarespebr](https://www.linkedin.com/in/gabrielsoarespebr/)
  - GitHub: [gabrielsoarespebr](https://github.com/gabrielsoarespebr)