# Robot arm grasping tasks
To further analyze the advantages of our method and the other two relatively well-performing baselines. We publish the video of their experiment here.
## Task description
The experiment involves a 6-DoF robot arm performing grasping tasks within a $30\times30\times30cm^3$ tabletop workspace. $15$ rounds of experiments are conducted using our method and baselines. In each round, $6$ objects are randomly selected and placed on the table. The robot observes the workspace with a single-depth image from a fixed side view. The viewpoint of the virtual camera points toward the workspace's origin at a radial distance $r=2l$ and an angle $\theta=\pi/3$, $l$ is the workspace's length. We set the total number of interactions to 6. Thus, the robot arm is allotted a single observation of the environment per object. The robotic arm has to first acquire observations at the beginning of each grasping. Upon perceiving the observation, a fixed-length action sequence is executed to grasp the target object and then place the object in the target box. The time limit for grasping one object is set to $30s$. 
## Videos of methods
Three experiment videos are provided.
- Our method: MARS + TD3-BC
- Baseline 1: Multistep + TD3-BC
- Baseline 2: Dense obs + TD3-BC
## Analysis
Our MARS + TD3-BC demonstrates strong ability in efficiently accomplishing the grasping task within each fixed interaction interval, whereas the Multistep + TD3-BC falls in grasping two small objects. Dense obs + TD3-BC performs the worst even unable to successfully grasp the larger beverage bottles.
