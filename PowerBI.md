# PowerBI

### Drill Through

- [Create Buttons](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-drill-through-buttons)
- [Pages](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-drillthrough)
- The Feature

### Formatting Strings & Numbers

1. Format Function [MS](https://learn.microsoft.com/en-us/dax/format-function-dax) / [SQLBI](https://dax.guide/format/)
2. Dynamic Formatting:
   1. Use the field formating function in PowerBI
   2. [Dynamic Formatting Strings for Measures](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-dynamic-format-strings) / [video](https://www.youtube.com/watch?v=a3D7oXYjM9k)

|         number | formatting string |        results | remarks                                                            |
| -------------: | ----------------: | -------------: | :----------------------------------------------------------------- |
| 01 234 567.210 |    ##,###,###.### |   1,234,567.21 | # is a optional placeholder                                        |
| 01 234 567.210 |    00,000,000.000 | 01,234,567.210 | 0 is a mandatory placeholder                                       |
|           0.45 |               0.0 |            0.5 | the missing digit rounds the last decimal                          |
|           0.45 |               #.0 |             .5 | the # is optional                                                  |
| 01 234 567.210 |         00,000,.0 |       01,234.6 | ,. skips the last x1000 and rounds it as a decimal                 |
| 01 234 567.210 |       00,000,.0 k |     01,234.6 k | ,. skips the last x1000 and rounds it as a decimal and add the "k" |
| 01 234 567.210 |           00,,.00 |          01.23 | ,,. skips the last x1 000 000 and rounds it as a decimal           |
| 01 234 567.210 |        ##0,,.00 M |         1.23 M | The M is added as a millions indicator                             |

source: [Display Formatting Strings](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-custom-format-strings) / [video](https://www.youtube.com/watch?v=FVjtWouD5Fw)

### Currencies

1. https://gist.github.com/voskobovich/43f851859c23a8261514

### Conditional Formatting

1. [Hevo](https://hevodata.com/learn/power-bi-conditional-formatting/#2)

**_Snippets_**

1. [DAX snippets](.\Snippets\DAX\)

### Localization in PowerBI, Excel & Windows

1. [Format Functie in PowerBI](https://learn.microsoft.com/en-us/dax/format-function-dax)
2. [Country Region and Language Codes](https://support.microsoft.com/en-us/topic/country-region-and-language-codes-add36afe-804a-44f1-ae68-cfb9c9b72f8b)
3. [Windows Locale support](https://learn.microsoft.com/en-us/windows/win32/api/winnls/nf-winnls-localenametolcid)
4. [Create **Dynamic Format Strings**](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-dynamic-format-strings)
   1. [Use Dynamic Format Strings](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-custom-format-strings)
   2. [5 Techniques: Basic to Advanced - YouTube ](https://www.youtube.com/watch?v=4HfKHYX_nHo)

| Country        | Currency |     Format |
| :------------- | :------- | ---------: |
| Australia      | Dollar   | AU$ #,0.00 |
| Canada         | Dollar   |  C$ #,0.00 |
| Denmark        | Krone    |     kr #,0 |
| Euro Zone      | Euro     |   € #,0.00 |
| Japan          | Yen      |      ¥ #,0 |
| Sweden         | Krona    |     kr #,0 |
| Switzerland    | Franc    | CHF #,0.00 |
| United Kingdom | Pound    |      £ #,0 |
| United States  | Dollar   | US$ #,0.00 |

1. [Drilltrough reports](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-drillthrough)

## Design

### Theming

1. [Power BI Theming](https://learn.microsoft.com/en-us/power-bi/connect-data/desktop-python-scripts)
2. [!YT](https://youtu.be/ubk5smogosk)
