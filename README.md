📊 EMA Crossover Strategy (Python)

This project implements a basic Exponential Moving Average (EMA) crossover trading strategy using Python.
The strategy generates long and short signals based on EMA crossovers, and visualizes the entry points separately for clarity.

✅ Features

Synthetic price data simulation (trend + noise)

EMA(20) & EMA(50) crossover logic

Long entry chart — marks where long signals are generated

Short entry chart — marks where short signals are generated

Easy to convert to live market data (Stock/Crypto)

⚙️ Strategy Logic
Condition	Action
EMA(20) crosses above EMA(50)	Go Long (Buy)
EMA(20) crosses below EMA(50)	Go Short (Sell)
Signal change is detected using diff() on signal column.	

This project only marks entry points. Exit points are implied by opposite signals.

🧠 Concept
What is EMA?

EMA = Exponential Moving Average
It weights recent price more heavily than older prices → reacts faster than SMA.

Why EMA crossover?

It identifies trend reversals:

Fast EMA moves first

Slow EMA confirms long-term direction

Common usage in algo-trading, crypto bots, technical trading systems.

📦 Requirements
Install Dependencies
!pip install pandas numpy matplotlib

🧾 Usage
Run the script
python ema_strategy.py


Output:

Chart 1: Long entry points (▲ arrows)

Chart 2: Short entry points (▼ arrows)

First few rows of processed data

📈 Example Output

✔️ EMA plotted on price chart
✔️ Long/Short signals highlighted
✔️ Clear visual understanding of strategy behavior# EMA-strategy
