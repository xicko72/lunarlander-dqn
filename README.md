# LunarLander DQN

A Deep Q-Network (DQN) agent for Gymnasium’s `LunarLander-v3`. The PyTorch implementation uses a replay buffer, an epsilon-greedy policy and a softly updated target network. The notebook plots episode reward and training loss, then records videos of the trained policy.

## Run

Install Python dependencies with `pip install -r requirements.txt`. Box2D may also require SWIG and system build tools on your machine. Open `lunarlander_dqn.ipynb` in Jupyter and run the cells in order. Training defaults to 1,000 episodes and can take substantially longer than a few minutes on CPU; reduce `n_episodes` for a quick check. The plots and videos are generated locally and are not tracked here.

The notebook uses a fixed seed for Python, NumPy and PyTorch and seeds each training episode. Exact scores can still vary across platforms or library versions. No external dataset is required: observations and rewards come from the simulation. This is an experiment, not evidence of a solved environment without a fresh full run.
