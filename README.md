# Piperider Getting Started

This is the demo project for piperider getting started.


# Steps

1. Download the sqlite data

   ```bash
   curl -o data/sp500.db https://piperider-data.s3.ap-northeast-1.amazonaws.com/getting-started/sp500_20220401.db
   ```

1. Install piperider

   ```bash
   pip install piperider-cli
   ```

1. Run the piperider

   ```bash
   piperider-cli run --generate-report 
   ```

1. Open the piperider report files printed in the stdout.   

1. Download another sqlite data

   ```bash
   curl -o data/sp500.db https://piperider-data.s3.ap-northeast-1.amazonaws.com/getting-started/sp500_20220527.db
   ```

1. Run piperider again

   ```bash
   piperider-cli run --generate-report 
   ```

1. Compare two runs

   ```bash
   piperider-cli compare-report
   ```

   and select the runs you would like to compare
