# Football-Space-Dominance-Prediction
This project explores how Graph Neural Networks (GNNs) and Long Short-Term Memory (LSTM) models can predict future space dominance in football using real-world tracking data. While traditional models like Voronoi diagrams capture static control of space, this project takes it further by forecasting which player will dominate each area of the pitch up to 3 seconds ahead, based on a 6-second input window.

Core Highlights:
- Input: 5Hz tracking data (x, y coordinates, velocity, team/player IDs, ball position).
- Model: A GNN models spatial interactions between players, while an LSTM captures movement patterns over time.
- Output: A 100x64 grid predicting per-player space dominance (based on Voronoi-style labels).
- Result: Achieved a strong mean Intersection over Union (mIoU) of 0.8362, confirming the model’s ability to generalize across player roles and game contexts.
- Sensitivity-tested: Robust to small positional and velocity changes, and interpretable in tactical contexts.

Why It’s Useful:
- Offers forward-looking spatial analysis for tactical planning, player evaluation, and real-time coaching.
- Moves beyond static snapshots—modeling how control evolves, not just where it is.
- Can be integrated into scouting tools, broadcast analytics, or simulation environments.
