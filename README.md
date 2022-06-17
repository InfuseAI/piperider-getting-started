# Piperider Getting Started

This is the getting started project for [piperider](https://github.com/InfuseAI/piperider)

# Steps

1. Clone the project

   ```bash
   git clone https://github.com/InfuseAI/piperider-getting-started.git
   cd piperider-getting-started/
   ```

1. Install piperider

   ```bash
   pip install -U piperider
   ```

1. Download the sqlite data

   ```bash
   curl -o data/sp500.db https://piperider-data.s3.ap-northeast-1.amazonaws.com/getting-started/sp500_20220401.db
   ```

1. Init a piperider project. 

   <details>
    <summary>You can skip this step because this is already a piperider project. If you would like to try to init the project on you own, you can try this</summary>

    ```bash
    rm -rf .piperider/
    piperider init   
    ```

    Input these options 
   
    - **project name**: demo
    - **data source type**: sqlite
    - **path to database file**: data/sp500.db

   </details>   

1. Diagnose if the data source is well-configured

   ```
   piperider diagnose
   ```

1. Run the piperider

   ```bash
   piperider run --generate-report 
   ```

1. Open the piperider report files printed in the command output

1. Download another sqlite data

   ```bash
   curl -o data/sp500.db https://piperider-data.s3.ap-northeast-1.amazonaws.com/getting-started/sp500_20220527.db
   ```

1. Run piperider again

   ```bash
   piperider run --generate-report 
   ```

1. Compare two runs

   ```bash
   piperider compare-report
   ```

   and select the reports you would like to compare
