# 📊 Excel Cheat Sheet: Zero to Mastery

> Brackets surrounding an argument in function syntax (e.g., `[argument]`) indicate that the argument is optional.

---

## 📅 Date & Time Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `DATE` | Returns a date based on inputs of year, month, and day. | `DATE(year, month, day)` |
| `DATEDIF` | Calculates the number of days, months, or years between two dates. | `DATEDIF(start_date, end_date, unit)` |
| `DAY` | Converts a date value to a day of the month. | `DAY(serial_number)` |
| `EOMONTH` | Returns the last day of the month before/after a specified number of months. | `EOMONTH(start_date, months)` |
| `MONTH` | Converts a date value to a month. | `MONTH(serial_number)` |
| `NETWORKDAYS` | Returns the number of whole workdays between two dates. | `NETWORKDAYS(start_date, end_date, [holidays])` |
| `NOW` | Returns the current date and time. | `NOW()` |
| `TODAY` | Returns today's date. | `TODAY()` |
| `WEEKDAY` | Converts a date value to a day of the week. | `WEEKDAY(serial_number, [return_type])` |
| `YEAR` | Converts a date value to a year. | `YEAR(date_value)` |

---

## 💰 Financial Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `FV` | Returns the future value of an investment. | `FV(rate, num_periods, payment, [present_value], [type])` |
| `PMT` | Calculates loan payments. | `PMT(rate, num_periods, present_value, [future_value], [type])` |

---

## ❓ Information Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `ISBLANK` | Checks whether a value is blank. | `ISBLANK(value)` |
| `ISERROR` | Checks whether a value is an error. | `ISERROR(value)` |
| `ISNUMBER` | Checks whether a value is a number. | `ISNUMBER(value)` |

---

## 🧩 Logical Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `AND` | Returns TRUE if all arguments are TRUE. | `AND(logical1, logical2, ...)` |
| `IF` | Returns one value if condition is met, another if not. | `IF(logical_test, value_if_true, value_if_false)` |
| `IFERROR` | Handles formula errors gracefully. | `IFERROR(value, value_if_error)` |
| `NOT` | Inverts TRUE/FALSE. | `NOT(logical)` |
| `OR` | Returns TRUE if any argument is TRUE. | `OR(logical1, logical2, ...)` |

---

## 🔍 Lookup Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `HLOOKUP` | Searches top row for a match and returns a value from a specified row. | `HLOOKUP(lookup_value, table_array, row_index_num, [range_lookup])` |
| `INDEX` | Returns a value from a range based on position. | `INDEX(array, row_num, [column_num])` |
| `MATCH` | Returns the relative position of a matching item. | `MATCH(lookup_value, lookup_array, [match_type])` |
| `VLOOKUP` | Searches first column for a match and returns a value from a specified column. | `VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])` |

---

## ➕ Mathematical Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `ABS` | Returns the absolute value of a number. | `ABS(number)` |
| `MOD` | Returns the remainder after division. | `MOD(number, divisor)` |
| `ROUND` | Rounds a number to a specified number of digits. | `ROUND(number, num_digits)` |
| `ROUNDDOWN` | Rounds a number down toward zero. | `ROUNDDOWN(number, num_digits)` |
| `ROUNDUP` | Rounds a number up away from zero. | `ROUNDUP(number, num_digits)` |
| `RAND` | Returns a random real number between 0 and 1. | `RAND()` |
| `RANDBETWEEN` | Returns a random integer between two integers. | `RANDBETWEEN(bottom, top)` |
| `SUM` | Adds all numbers in a range. | `SUM(number1, [number2], ...)` |
| `SUMIF` | Sums values that meet criteria. | `SUMIF(range, criteria, [sum_range])` |
| `SUMIFS` | Sums values that meet multiple criteria. | `SUMIFS(sum_range, criteria_range1, criteria1, [criteria_range2, criteria2], ...)` |
| `SUMPRODUCT` | Returns sum of products of corresponding ranges. | `SUMPRODUCT(array1, [array2], [array3], ...)` |

---

## 📈 Statistical Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `AVERAGE` | Returns average of values. | `AVERAGE(number1, [number2], ...)` |
| `AVERAGEIF` | Returns average of cells that meet criteria. | `AVERAGEIF(range, criteria, [average_range])` |
| `AVERAGEIFS` | Returns average of cells that meet multiple criteria. | `AVERAGEIFS(average_range, criteria_range1, criteria1, [criteria_range2, criteria2], ...)` |
| `COUNT` | Counts numeric values in list. | `COUNT(value1, [value2], ...)` |
| `COUNTA` | Counts non-blank values in list. | `COUNTA(value1, [value2], ...)` |
| `COUNTBLANK` | Counts empty cells in a range. | `COUNTBLANK(range)` |
| `COUNTIF` | Counts cells that meet criteria. | `COUNTIF(range, criteria)` |
| `COUNTIFS` | Counts cells that meet multiple criteria. | `COUNTIFS(criteria_range1, criteria1, [criteria_range2, criteria2], ...)` |
| `MAX` | Returns maximum value. | `MAX(number1, [number2], ...)` |
| `MEDIAN` | Returns median of given numbers. | `MEDIAN(number1, [number2], ...)` |
| `MIN` | Returns minimum value. | `MIN(number1, [number2], ...)` |
| `STDEV.P` | Returns standard deviation of population. | `STDEV.P(number1, [number2], ...)` |

---

## ✍️ Text Functions

| Function | Description | Syntax |
|---------|-------------|--------|
| `CONCATENATE` | Joins two or more text strings. | `CONCATENATE(text1, [text2], ...)` |
| `FIND` | Returns starting position of one string within another. | `FIND(find_text, within_text, [start_num])` |
| `LEFT` | Returns leftmost characters from a text string. | `LEFT(text, [num_chars])` |
| `LEN` | Returns number of characters in a text string. | `LEN(text)` |
| `LOWER` | Converts text to lowercase. | `LOWER(text)` |
| `MID` | Returns specific characters from a text string. | `MID(text, start_num, num_chars)` |
| `PROPER` | Capitalizes first letter of each word. | `PROPER(text)` |
| `RIGHT` | Returns rightmost characters from a text string. | `RIGHT(text)` |
| `SUBSTITUTE` | Substitutes new text for old text. | `SUBSTITUTE(text, old_text, new_text, [instance_num])` |
| `TEXT` | Changes how a number appears using format codes. | `TEXT(value, text_format)` |
| `TRIM` | Removes extra spaces from text. | `TRIM(text)` |
| `UPPER` | Converts text to uppercase. | `UPPER(text)` |

---

## 🎯 Handy Formula Recipes

| Scenario | Formula |
|---------|---------|
| Dynamically calculate a date 3 months from today | `=DATE(YEAR(TODAY()), MONTH(TODAY())+3, DAY(TODAY()))` |
| Return the first day of the current month | `=EOMONTH(TODAY(),-1)+1` |
| Error-proof VLOOKUP | `=IFERROR(VLOOKUP(A2,Sheet2!A:B,2,FALSE),"Value not found")` |
| "Found" or "Not Found" check | `=IF(ISERROR(MATCH("Excel",A:A,0)),"Not found","Found")` |
| Multi-level classification (High/Medium/Low) | `=IF(A1>1000,"High",IF(A1>=200,"Medium","Low"))` |
| Complex logic with AND | `=IF(AND(A1>1000000,B1>20),"Yes","No")` |
| Two-way lookup with INDEX + MATCH | `=INDEX(A1:J10,MATCH("Excel",A1:A10,0),MATCH("Travis",A1:J1,0))` |
| Random sample with RANDBETWEEN + INDEX | `=INDEX(A1:A10,RANDBETWEEN(1,10))` |
| Get current day name | `=TEXT(TODAY(),"dddd")` |
| Extract first name from full name | `=LEFT(A1,FIND(" ",A1)-1)` |
| Remove periods and commas from text | `=SUBSTITUTE(SUBSTITUTE(A1,".",""),",","")` |

---

## ⚠️ Common Formula Errors

| Error | Meaning |
|-------|---------|
| `#DIV/0!` | Division by zero |
| `#NAME?` | Unrecognized function or name |
| `#VALUE!` | Incorrect data type used |
| `#REF!` | Invalid reference (e.g., deleted cell) |
| `######` | Column too narrow to show value |

---

## 🌟 Final Tips

- Use **keyboard shortcuts** like `Ctrl + Shift + Arrow` to navigate quickly.
- Press `F9` to recalculate formulas manually.
- Combine **INDEX + MATCH** instead of VLOOKUP for more flexibility.
- Always **wrap lookups in IFERROR** to avoid ugly errors.

---
