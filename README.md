A daily performance tracker for the self-made protocol (smp) fitness program.
Logs sleep, water intake, and steps count. Predict goal achievements using a trained Random Forest Classifier and generates a coaching message.
            What it does
- Accepts daily check-in data (sleep hours,water glasses,steps)
- Predicts whether the 10,000-steps goal will be hit
- Returns a confidence score and a direct coaching message
- Export a weekly summary report as JSON.
               SETUP
  pip install -r requirements.txt
            USAGE
  from coaching import analyze_day(sleep=7.5,water_glasses=9,bench_kg=8.8)
  print(result[coaching])
          SAMPLE OUTPUT
  Prediction: Hit goal(88% confidence)
  Coach: Strong inputs, strong outputs. Baseline is locked in.
            STACK
  .Python   . Scikit-learn  . Pandas  .FastAPI
