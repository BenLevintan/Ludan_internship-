# Google Sheets Custom Functions for Construction Project Management

This repository contains JavaScript functions developed during my internship at Ludan Group. These functions were designed to enhance the management of project documentation for a construction project using Google Sheets. By automating color-based cell counting and retrieval, these functions streamline progress tracking and data categorization, significantly improving workflow efficiency.

## Functions

### `countColor(sheetName, column, colorName)`
Counts the number of cells with a specified background color in a given column.

#### Parameters:
- `sheetName` (string): The name of the sheet to search in.
- `column` (string): The column to count colored cells in (e.g., `"A:A"`).
- `colorName` (string): The color to count. Accepted values: `"green"`, `"orange"`, `"gray"`, `"purple"`.

#### Returns:
- `number`: The count of cells with the specified background color.

#### Example Usage:
```javascript
const count = countColor("Sheet1", "A:A", "green");
Logger.log(count);  // Outputs the count of green-colored cells in column A
