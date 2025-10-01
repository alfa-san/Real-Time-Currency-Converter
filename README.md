# 💲 Real-Time Currency Converter

An advanced Excel-VBA tool designed for real-time and historical currency conversion. It features a user-friendly interface powered by a custom VBA User Form.

## 🧩 Business Problem
The need for a reliable tool to convert currency using real-time and historical exchange rates, while also providing visual data on market trends.

## 🚀 Key Features
- **Real-Time Data Query**: Automatically fetches up-to-date exchange rates for accurate conversions
- **Historical Data**: Retrieve past exchange rates for a specific date
- **Visualization**: Plot exchange rate trends over a user-defined time window

## 🛠 Skills Used
- VBA Programming: User Forms, Modules, Error Handling, Sub/Function procedures
- Data Automation: Querying external sources
- Data Visualization: Dynamic chart generation in Excel
- Excel Functions: Supporting calculations and formatting

## 📦 File Contents
- `Real-Time-Currency-Converter_v0.1.0.xlsm` – Main Excel macro-enabled file
- `README.md` – Project documentation
- `CHANGELOG.md` – Version history and feature log

## 📜 Version History

This project now follows [Semantic Versioning](https://semver.org/).  
See [`CHANGELOG.md`](CHANGELOG.md) for detailed updates.

Current version: `v0.1.0`

## 📚 Usage

1. **Unblock the file**:  
   After downloading the `.xlsm` file from the internet, right-click the file, select **Properties**, and under the **General** tab, check the **Unblock** box. Click **OK** to apply.

2. **Enable macros**:  
   Open the `.xlsm` file in Microsoft Excel and enable macros when prompted to allow the VBA code to run.

3. **Run Currency Converter**:  
   In the `Currencies` sheet, there is a list of currencies and the `Run Currency Converter` button. Click the button to run converter.
   - Convert different currencies
   - Change exchange rate dates
   - Plot in days

4. **Exit safely**:  
   Use the **Quit** button to close the form and return to the workbook.

## 🧪 Limitations & Future Improvements

This tool is actively being improved. Known limitations include:
- **Slow performance in querying of data from web**: 
  Querying data is less than optimal. Need to speed up data retrieval.

- **Slow performance when plotting multiple days**:  
  Querying and visualizing large sets of exchange rate data can be slow. Optimization is needed to speed up data retrieval and chart rendering.

- **Web query dependency**:  
  Relies on [xe.com](https://www.xe.com) structure, which may change and break the query logic.

- **Limited caching support**:  
  The tool stores the most recently fetched exchange rate data in a hidden sheet, which is used as the default reference on subsequent runs. However, it does not maintain a broader cache or allow offline access to historical data. Upon opening the workbook, the tool automatically updates to the previous day's rates (Current Date - 1) to ensure fresh data.

Planned enhancements:
- Investigate faster data sources or caching strategies
- Refactor plotting logic for better performance
- Improve error handling for edge cases in historical queries


## 📬 Feedback & Contributions
Feel free to fork, improve, or suggest enhancements via GitHub Issues or Pull Requests.