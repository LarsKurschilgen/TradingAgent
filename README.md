# TradingAgent
## Description
Within this project, a Trading Agent is developed to learn how to trade the Apple stock. The agent can perform three actions: Hold, Buy, and Sell. The goal of the agent is to make trading decisions and exploit price fluctuations like a trader.

### Environment

The custom trading environment `CustomTradingEnv` is defined using the `gym` library. To adapt it for the application case, the following main components were fundamentally defined:

- **Action Space**: The agent can perform three actions: Hold, Buy, and Sell.
- **Observation Space**: The agent observes a window of market data, scaled to the range [0, 1].
- **Reward Function**: Rewards are calculated based on the agent's actions and market price changes, considering transaction costs.
- **State Management**: The environment maintains the current step, position, total profit, and trade history.
  
### Agent

The agent used in this project is based on a Double Deep Q-Network. The implementation is adapted from the repository [Super-Mario-Bros-RL](https://github.com/Sourish07/Super-Mario-Bros-RL). Several modifications were made to tailor it to the project's requirements:

- **A different neural network architecture was used, incorporating LSTMs.**
- **Adjustments were made to other parts of the code to support the new architecture and the specific needs of this project.**

## Requirements
1. Clone Repository
2. Create a virtual python environment
3. Install required packages listed in [requirements.txt](https://github.com/LarsKurschilgen/TradingAgent/blob/main/requirements.txt)
