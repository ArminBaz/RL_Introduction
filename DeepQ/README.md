# Deep Q Learning
Implemented using OpenAI gym and Keras

## Introduction:
This was done as a project in order to become a membor of Professor Tao Gao's lab at UCLA.
This is a relatively simplistic implementation, however it does a pretty good job.

## Testing:
Thus far I have only tested it on the CartPole-V1 environment provided via OpenAI's gym.

### Results
I trained the CartPole for 600 episodes. The first jump in score occurred around episode 115, where the agent would consistently score above 30-40 points. The second jump in score was on episode 141 where the agent broke a score of 100.

Once the number of episodes got into the 300 range, the agent became good. Mastery occurred in the early to mid 400's.

As far as the network itself. My architecture was very simple. One input layer, two hidden layers, one output layer. At first, I used a layer size of 128 for the hidden layers, this yielded good results however training was slow.

I then used layer sizes of 32 and 64 and was rewarded with much faster training and similar results. I think due to the simplistic nature of this problem, larger hidden layers is unnecessary.

## Future Work:
- There was a very interesting article: http://inoryy.com/post/tensorflow2-deep-reinforcement-learning/ made by a researcher at DeepMind. He implemented an actor critic method using deep learning, could be worthwhile to look into and compare results with.
- Test Model on different environments
- Test out different versions of DQL Networks (Weighted Q Learning, Multiple Agents, Two Network Model, etc.)

