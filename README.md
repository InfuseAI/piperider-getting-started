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
   piperider run --generate-report 
   ```

1. Open the piperider report files printed in the stdout.   

