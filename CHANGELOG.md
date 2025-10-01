# 📄 CHANGELOG.md

All notable changes to this project will be documented in this file.  
This project follows [Semantic Versioning](https://semver.org/).

---

## [v0.1.0] – 2025-10-01

### 🚀 Added
- Initial development release of **Real-Time Currency Converter**
- Custom VBA User Form for intuitive currency conversion
- Real-time exchange rate retrieval using web query from [xe.com](https://www.xe.com)
- Historical rate lookup by user-specified date
- Dynamic chart generation to visualize exchange rate trends over a selected number of days
- Currency swap functionality. Allows users to reverse the selected currency pair in the ComboBoxes (e.g., swap USD to EUR → EUR to USD)
- Error-handling routine for failed web queries
- README documentation with onboarding instructions

### 🧪 Known Limitations
- **Slow performance in querying of data from web**: 
  Querying data is less than optimal. Need to speed up data retrieval.

- **Slow performance when plotting multiple days**:  
  Chart generation and data retrieval can be sluggish, especially for longer time windows. Optimization is needed to improve speed.

- **Web query dependency**:  
  Relies on [xe.com](https://www.xe.com) structure, which may change and break the query logic.
  
- **Limited caching support**:  
  The tool stores the most recently fetched exchange rate data in a hidden sheet, which is used as the default reference on subsequent runs. However, it does not maintain a broader cache or allow offline access to historical data. Upon opening the workbook, the tool automatically updates to the previous day's rates (Current Date - 1) to ensure fresh data.

### 📌 Notes
- This version is marked as a **pre-release** and is not yet production-ready.
- Future improvements will focus on performance, robustness, and enhanced visualization.

