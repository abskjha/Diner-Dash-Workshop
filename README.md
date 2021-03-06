# **Reinforcement Learning: DinerDash challenge**

## Overview
This workshop provides an interactive avenue for participants to learn about Reinforcement Learning (RL). Diner Dash is a game where a single waiter makes complex decisions on customer seating arrangements, taking orders, serving food and many others. In groups of 2 or 3, participants would test out RL baselines and compete with one another for the highest score in the Diner Dash simulator. 

## Official Schedule
#### 4 August 2020, Tuesday (GMT +8)
| **Time** | **Programme** |
| - | - |
| 9am | [Introduction to Reinforcement Learning](#Introduction-to-Reinforcement-Learning) |
| 10am | [Diner Dash Introduction](#Diner-Dash-Introduction) |
| 10:30am | [Diner Dash Challenge Briefing](#Diner-Dash-Challenge) |
| 11am | [Start of Challenge](#Diner-Dash-Challenge) |
| 4pm  | [Random seeds given for testing,](#Random-seeds) [Submission platform opens](#Submission-platform) |
| 9pm  | Cut off for submissions |

#### 6 August 2020, Thursday (GMT +8)
| **Time** | **Programme** |
| - | - |
| 5pm | [Award Presentation](#Award-Presentation) |

## Introduction to Reinforcement Learning
Speaker: [Akshay Narayan](https://www.comp.nus.edu.sg/cs/bio/anarayan/)

This is an introductory talk on reinforcement learning (RL). In this talk, we will introduce the vocabulary of RL, cover the basics of sequential decision making and RL. We will touch upon value function based and policy search methods for solving RL problems. We will look at some applications and limitations of RL.

## Diner Dash Introduction
Author of the Diner Dash Simulator: Siwei

Siwei will introduce the features and background of the DinerDash simulator as well as some of the challenges and difficuties one may face when training our agent.

Please refer to the [diner dash repo](https://github.com/AdaCompNUS/diner-dash-simulator) for more information.

## Diner Dash Challenge
### Prerequisites
- Basic knowledge of Python
- A stable internet connection
- A Google account
- A GitHub account
- A zoom account

### Objective
Using Reinforcement Learning(RL) algorithms and a **maximum training timestep of 10 million**, maximise the average rewards from 100 games/episodes of Diner Dash.

### Challenge Platform
We will be using Google Colab for this challenge. The challenge template and further instructions are provided [here](https://github.com/AISG-Technology-Team/Diner-Dash-Workshop/blob/master/Challenge_Template.ipynb). Please open the notebook in colab and create a copy in your Google Drive.

### Random seeds
100 random seeds would be uploaded to this repo as per the [official schedule](#Official-Schedule). Each seed is used to initialise an environment/game where trained models decide on the action to take to maximises rewards. The list of actions taken is returned for submission.

Please see the "Testing of Policies and Verification of Submission" section in the [template notebook](https://github.com/AISG-Technology-Team/Diner-Dash-Workshop/blob/master/Challenge_Template.ipynb) for an example of how to use the random seeds.

A sample list of random seeds can also be found [here](https://github.com/AISG-Technology-Team/Diner-Dash-Workshop/blob/master/sample_randomSeeds.py).

### Submission Format
Please choose **both files** before submitting:
- Google Colab Notebook (.ipynb)
    - Filled with Team Name, Team ID, names of group members and algorithms used
    - Please ensure that the notebook is ran and displays training outputs
    - Action lists in notebook must match the submitted json file
- Json file (.json)
    - With lists of actions in order of random seeds
        ```
        # [6, 45, 32, 53, 4] corresponds to the first seed
        # [27, 3, 12, 34, 1, 18]] corresponds to the second seed
        # The list of actions do NOT have to be the same length
        {
            "randomAgent": 
                [[6, 45, 32, 53, 4],
                [27, 3, 12, 34, 1, 18]],
        }
        ```

A sample submission can be found [here](https://github.com/AISG-Technology-Team/Diner-Dash-Workshop/tree/master/sample_submission).

### Submission platform
Each participant should receive a link via email for submission and viewing of the leaderboard. Please keep this link private and do not share it with others. If you face any difficulty in using the link, please contact [Lin Xu](mailto:linxu@aisingapore.org).

Alternatively, the leaderboard can be viewed at this [link](https://aisummerschool.aisingapore.org/submission) as well.

### Submission rules
- Each group can only submit a maximum of 5 submissions
- Only the best performing submission per group would be kept and ranked in the leaderboard. However, please double check the average rewards before submitting to ensure that subsequent submissions perform better than the previous.

### Submission dateline
Cut off time for submission is as per the [official schedule](#Official-Schedule)

### Question and Answer
We will be using this repo's [issues](https://github.com/AISG-Technology-Team/Diner-Dash-Workshop/issues) for question and answer. Please discuss within your group first and if the query is still unresolved, check if a relevant issue has been raised. If none exist, please raise a new issue. Feel free to answer other participants' queries as well if you have faced similar issues and found a resolution.

## Award Presentation
The top 3 ranking teams would present their approach and learning points. Certificates would also be awarded to them for their achievements.

## Additional Resources
- [RL Stable Baselines Repo](https://github.com/hill-a/stable-baselines)
- [RL Stable Baselines Tutorial + Colab Notebooks](https://github.com/araffin/rl-tutorial-jnrr19)
- [DinerDash Gym: A Benchmark for Policy Learning in High-Dimensional Action Space](https://github.com/AISG-Technology-Team/Diner-Dash-Workshop/blob/master/DinerDash%20Gym_%20A%20Benchmark%20for%20Policy%20Learning%20in%20High-Dimensional%20Action%20Space.pdf)
- [Deep Q-learning (DQN) Tutorial](https://www.analyticsvidhya.com/blog/2019/04/introduction-deep-q-learning-python/)
- [RL Library for tensorflow](https://github.com/tensorflow/agents): [TF agent DQN Tutorial](https://github.com/tensorflow/agents/blob/master/docs/tutorials/1_dqn_tutorial.ipynb)

## Acknowledgements
### Tutorial Speaker
- [Akshay Narayan](https://www.comp.nus.edu.sg/cs/bio/anarayan/)

### Diner Dash Simulator
- Siwei

### AI Singapore (Organisers)
- Dr Winkler
- Benjamin Chua
- Lin Xu
- Haixun
- Sean

[Back to top](#reinforcement-learning-dinerdash-challenge)