# RNN Assignment Project

This project covers the assignment's five parts:

- **Part A:** Simple RNN temperature prediction using the Jena Climate dataset, sliding windows, normalization, hyperparameter experiments, MAE/MSE/RMSE, and plots.
- **Part B:** IMDB sentiment classification with trainable embeddings (dimensions 32, 64, 128), classification metrics, and confusion matrix.
- **Part C:** Simple RNN vs LSTM vs GRU comparison, parameter counts, training time, and an example LSTM hidden/cell-state plot.
- **Part D:** Small English-to-French encoder-decoder demonstration with `<START>` / `<END>` tokens, ten held-out examples, and BLEU scores.
- **Part E:** Integrated analysis and limitations in the report.

## Run it (Windows / VS Code)

1. Install Python 3.10+.
2. Extract this folder and open it in VS Code.
3. Open **Terminal → New Terminal**.
4. Create a virtual environment:

   ```powershell
   py -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

5. Install dependencies:

   ```powershell
   python -m pip install -r requirements.txt
   ```

6. Run the project:

   ```powershell
   python rnn_assignment.py
   ```

For a quicker test with smaller samples and fewer epochs:

```powershell
python rnn_assignment.py --quick
```

The script downloads the Jena Climate and IMDB datasets when first needed. Internet access is required. Output tables and charts are saved in `results/`.

## Important notes

- The small translation corpus is for demonstrating the encoder-decoder mechanics only. It is not suitable for judging real-world translation quality.
- Results depend on your machine, package versions, random initialization, and training settings. Use the actual generated CSVs and plots in your report rather than copying results from another person's report.
- This is an educational assignment, not a production forecasting or translation system.
