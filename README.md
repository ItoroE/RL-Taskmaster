# Taskmaster

Taskmaster is a reinforcement learning-based task scheduler designed for an online setting where tasks arrive over time and their true durations are initially unknown.

The agent learns how long different types of tasks are likely to take and where new tasks should be placed within an existing schedule. The model combines **Proximal Policy Optimization (PPO)** with a **Pointer Network** to learn its scheduling policy.

## How It Works

- Tasks are generated over time with varying durations, deadlines, and rewards.
- The agent maintains a schedule and decides where to insert newly arriving tasks.
- A Pointer Network selects positions within the schedule.
- PPO is used to train the scheduling policy.
- The model also learns to predict task durations.

## Results

During training, the agent learns to leave gaps between scheduled tasks to account for possible future tasks while still filling available space when appropriate.

## Research Paper

For a full explanation of the problem, architecture, training process, results, and limitations, see the [Taskmaster Research Paper](research/Taskmaster_Final_Project.pdf).

## Authors

- Bryan Zhang
- Itoro Ekpenyong
- Jasamrit Rahala
