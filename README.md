# Portfolio-Performance

An Android application for stocks portfolio performance tracker built with Java 

## Usage Overview
User can input up to five stock tickers, and the relevant data between *July 1 2021, 00:00:01 to Dec 31 2021, 23:59:59* is gathered from [Finnhub](https://finnhub.io).

## Functionalities

Upon running the application in Android Studio, the main screen displays 5 text boxes to input stock tickers, and buttons on the bottom of screen indicating `Download` and `Calculate` respectively. 

Upon inputting valid stock tickers and clicking the `Download` and `Calculate` buttons in order, the application displays performance metrics measured namely, the annualised return and volatility of the respective stocks within the preset period.

Other than the above basic functionalities, the following are the extra quality of life features: 

- **Input Validation:** 

When an input ticker is invalid or empty, an error popup shows up on the corresponding text box.

- **Data Persistence:**

For power and computation efficiency, data for previously fetched tickers will not be redownloaded.

- **Error Prevention:**

The `Calculate` button will be inactive until the data for the ticker has been downloaded and persisted into the database.

- **Efficiency of Calculation:**

Each ticker is assigned a thread for its performance metrics calculation.

## How to run
1. Clone the repository on your local computer
2. Open the repository on Android Studio
3. Run the code and display using an emulator

Emulator recommended configuration :
  - Device: Nexus 6P
  - API: Level 30
  - Resolution: 1440 x 2560 (560 dpi)
  - Multi-Core CPU 4
  - RAM: 1536 MB
  - SD card: 512 MB

