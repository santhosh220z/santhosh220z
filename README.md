# Santhosh Sunkara

Applied ML engineer working on computer vision, deep reinforcement learning, and
the unglamorous parts of ML that decide whether a model is usable — serving it,
grading it, and keeping it honest about what it has actually measured.

**B.Tech, Computer Science (AI & ML), KIET — 2026.**

## Featured work

Six systems, each with a written blueprint — problem, approach, and the pipeline
it runs through.

| | Project | What it is |
| --- | --- | --- |
| 01 | [PyroGuard](https://github.com/santhosh220z/PyroGuard) | Real-time fire and smoke detection over camera streams. YOLOv8, with temporal verification so a single ambiguous frame cannot open an incident. FastAPI, pluggable alert providers behind a circuit breaker, SQLite incident lifecycle, Docker. |
| 02 | [Learn-to-drive-with-RL](https://github.com/santhosh220z/Learn-to-drive-with-RL) | PPO on Gymnasium `CarRacing-v3` from stacked grayscale frames. The point of the repo is the evaluation harness: held-out rewards written to `eval.json`, kept separate from the training reward, because only one of those two numbers is comparable across runs. |
| 03 | [code-and-algorithm-visualizer](https://github.com/santhosh220z/code-and-algorithm-visualizer) | Algorithms and data structures animated in lockstep with their own pseudocode, plus a mode that executes a program you paste in, line by line, with live variables and a recursive call stack. React 19, TypeScript. |
| 04 | [Deepfake-Detection](https://github.com/santhosh220z/Deepfake-Detection) | A served classifier for manipulated media: a Hugging Face checkpoint for stills, a GenConViT branch for video, behind a FastAPI endpoint that falls back to CPU. |
| 05 | [SIGN_SPEAK](https://github.com/santhosh220z/SIGN_SPEAK-The-Silent-Communicator) | Sign-language input turned into speech, for students who type to communicate and cannot. MediaPipe landmarks, a custom annotated dataset, temporal smoothing so the caption does not flicker. **Used by 50+ people**; selected for the regional round at TechSakshyam. |
| 06 | [StrokeSense](https://github.com/santhosh220z/ISCHEMIC_STOKE_PREDICTION) | Stroke risk from two inputs that never arrive together: a Random Forest over the clinical chart (SMOTE, `StratifiedKFold`) and a ResNet50V2 classifier for MRI, served by Flask to a React client. |

Also built: a
[stoichiometry engine](https://github.com/santhosh220z/CHEMICAL-REACTIONS-PROJECT)
that balances equations and resolves the limiting reagent from first principles,
and a
[disaster-response simulator](https://github.com/santhosh220z/disaster_management_simulation_using_RL)
where a Q-learning agent allocates beds, water and power — written directly
against NumPy with no RL framework.

## How I work

I am more interested in the part of a project after the notebook than before it.
Three things I have repeatedly reached for, each of them visible in the repos
above:

- **Refusing to act on weak evidence.** PyroGuard will not raise an alert on one
  frame, because a detector that pages on flicker teaches everyone to ignore it.
- **Measuring on held-out data.** The RL harness scores itself separately from
  its training reward; the clinical model is cross-validated with
  `StratifiedKFold` and oversampled with SMOTE, since raw accuracy on an
  imbalanced dataset is won outright by predicting the majority class.
- **Saying what is not done.** The RL repo records a passing smoke test and a
  training run still in progress rather than a reward it has not earned. PyroGuard
  carries an explicit notice that it is a prototype and not a certified
  fire-safety system.

## Stack

**Languages** Python, JavaScript, TypeScript, SQL

**ML** PyTorch, TensorFlow / Keras, Hugging Face Transformers, scikit-learn,
Stable-Baselines3, MediaPipe, OpenCV

**Ship** Docker, Docker Compose, FastAPI, Flask, Nginx, GitHub Actions, Render, Vercel

**Data** Pandas, NumPy, Streamlit, Plotly

## Currently

Looking for an entry-level AI/ML role — applied machine learning, computer
vision, or MLOps — where I can keep building with a team.

## Elsewhere

- Email — [santhoshsunkarasbe@gmail.com](mailto:santhoshsunkarasbe@gmail.com)
- LinkedIn — [siva-sambhavi-santhosh-sunkara](https://www.linkedin.com/in/siva-sambhavi-santhosh-sunkara-588a24265/)
