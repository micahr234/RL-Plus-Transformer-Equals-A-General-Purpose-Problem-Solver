# RL + Transformer = A General-Purpose Problem Solver

What if artificial intelligence could not only solve problems for which it was trained but also learn to teach itself to solve new problems (i.e., meta-learn)? In this paper, we demonstrate that a pre-trained transformer fine-tuned with reinforcement learning over multiple episodes develops the ability to solve problems that it has never encountered before—an emergent ability called In-Context Reinforcement Learning (ICRL). This powerful meta-learner not only excels in solving unseen in-distribution environments with remarkable sample efficiency, but also shows strong performance in out-of-distribution environments. In addition, we show that it exhibits robustness to the quality of its training data, seamlessly stitches together behaviors from its context, and adapts to non-stationary environments. These behaviors demonstrate that an RL-trained transformer can iteratively improve upon its own solutions, making it an excellent general-purpose problem solver.

<img src="https://github.com/user-attachments/assets/1149bcde-7c2f-4023-90e3-3b5fb5e2cb55" width="200"/>
<img src="https://github.com/user-attachments/assets/5266fe98-74ac-4ca1-98e1-5437f5ac0861" width="200"/>
<img src="https://github.com/user-attachments/assets/3359f7ab-34de-4755-b38f-e292cd5edc24" width="200"/>

In the plots above ICRL-trained Llama 3.1 learns to solve an unseen Frozen Lake environment. The trajectories in early, mid, and late interactions show solution refinement. Mistakes in early inference (e.g., falling into holes) disappear with experience in late inference.

This repository contains the code and experiments for our paper: **RL + Transformer = A General-Purpose Problem Solver**

## Overview

Our experiments show that an RL-trained transformer:

- Excels in solving unseen in-distribution environments with remarkable sample efficiency.
- Shows strong performance in out-of-distribution environments.
- Exhibits robustness to the quality of its training data.
- Seamlessly stitches together behaviors from its context.
- Adapts to non-stationary environments.


## Repository Structure

- `Train.ipynb`: Contains the implementation to ICRL train Llama.
- `Eval.ipynb`: Contains the implementation evaluate a trained model on new environments.
- `README.md`: Project overview and instructions.
- `LICENSE`: License information.


## Getting Started


### Prerequisites

- Python 3.8 or higher
- PyTorch
- Hugging Face Transformers
- Gymnasium (for environment simulations)


### Running Experiments


Fine-tune the pre-trained transformer with:

Train.ipynb - *make sure to add you huggingface username where appropriate*


Evaluate the trained model on new environments:

Eval.ipynb - *make sure to add you huggingface username where appropriate*


## Contact

For any questions or issues, please open an issue on this repository or contact us at:

- Micah Rentschler: [mrentschler@tntech.edu](mailto:mrentschler@tntech.edu)
- Jesse Roberts: [jroberts@tntech.edu](mailto:jroberts@tntech.edu)


