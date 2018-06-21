# Solve LunarLander problem by DQN
- The required codes(.py files) for this problem are:
```
LunarLander-DQN
│   README.md
│   p2.py    
│
└───variants
│   │   DQN.py
│   │   NavieDQN.py
|   |   DoubleDQN.py
|   |   DuelingDQN.py
|   |	PerDQN.py
│   │   
│   └───structure
│       │   neural_nets.py
│       │   replayD.py
│   
└───results
|   │   ...
|   │   ...
│   
└───dashboard
    │   ...
    │   ...
```

	  
- How to run:
  * The entry point main function is under p2.py
  * Run through commend line, need specify parameters, using (python p2.py --help) to see the description of the arguments
	* Training and save the result into "pkl" file:<br/>
		python p2.py  -analysis train -name NaiveDQN -alpha 5e-5 -gamma 0.99 -epsilon 2000<br/>
		once you finished training, you will have "pkl" files saved under results folder
	* Use the trained results pkl files to generate the plots for the report:<br/>
	    python p2.py  -analysis plot
  * alternatively, if you have a compiler, such as pyCharm, you can open p2.py, then execute the "execute_train_and_plt()" function

- If the python 3.5, tensorflow, OpenAI Gym, pybox2D, numpy, matplotlib already existed, please skip the following, otherwise, install them as below:
  - To compile the code, the python 3.5 is required<br/> 
    create a 3.5 virtual environment using anaconda:
    * conda create -n py35 python=3.5 anaconda
    * source activate py35
	 
  - The following platforms/libraries (tensorflow, Gym,pybox2d, numpy, matplotlib), must be available using the follwing commands:  
    * conda install -c conda-forge tensorflow
	* pip install gym
	* pip install box2d box2d-kengz (you may also need to install swig: conda install -c anaconda swig and vs2015: conda install -c anaconda vs2015_runtime)
	* conda install -c anaconda numpy 
    * conda install -c conda-forge matplotlib
   
