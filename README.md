# DRLND_3nd_project_FINAL
The submission version of DRLND 3nd project (collaboration and competition) solved with DDPG.
![](tennis_trained_result.gif) 
## Environment

### 1) States
* Vector observation space size is 24
* State space is consisted with (racket position x, y, velocity x, y, ball position x, y, velocity x, y) for three time steps
   *hence 8x3 = 24*
   

### 2) Actions
* Action size is 2 (*go towards (or away from) net / jump*)

### 3) Reward
* Reward +0.1 is given for each time the ball goes over the net.
* The episode ends when the ball touches the net or goes out of the court.
* Environment is considered solved when the average reward for 100 episodes becomes larger than 0.5.
* Since there are two different rewards (for each agent), the max reward is considered to be the actual reward.

## Getting Started

### 1) Instruction for Installing Dependencies

```
tensorflow==1.7.1
Pillow>=4.2.1
matplotlib
numpy>=1.11.0
jupyter
pytest>=3.2.2
docopt
pyyaml
protobuf==3.5.2
grpcio==1.11.0
torch==0.4.0
pandas
scipy
ipykernel
```

* from unityagents import UnityEnvironment
* env = UnityEnvironment(file_name='/data/Reacher_Linux_NoVis/Reacher.x86_64')

### 2) How to Run Code
* Run Jupyter notebook 'Tennis.ipynb' for both training and saving after problem is solved.

