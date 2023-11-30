# PowerBI

## General


[Optimizing](https://learn.microsoft.com/en-us/power-bi/guidance/)

## Making Reports

### Drill Through

- [Create Buttons](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-drill-through-buttons)
- [Pages](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-drillthrough)

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

**_Visualisation, Design, UI & UX_**

1. [Power BI visuals documentation](https://learn.microsoft.com/en-us/power-bi/developer/visuals/)
2. [GitHub Dataviz](https://github.com/bkrsln/dataviz)
3. [HTML5 Tags in tags](https://bisamurai.com/custom-visuals-knowledge-base/bold-italic-underline-power-bi/)
4. [Claus Wilke](https://clauswilke.com/dataviz/index.html)
5. Dashboard voorbeelden [Pinterest](https://www.pinterest.com/search/pins/?q=dashboard&rs=typed) / [FreePik](https://www.pinterest.com/search/pins/?q=dashboard&rs=typed) / [Adobe](https://stock.adobe.com/nl/search?k=Dashboard+&search_type=usertyped)
6. WireFraming and Mockups [Figma](https://www.figma.com/)
7. YT! [Guy In A Cube](https://www.youtube.com/watch?v=zaFTAT6_jCs) / [DataPears](https://www.youtube.com/@datapears) / [How to Power BI](https://www.youtube.com/@HowtoPowerBI)
8. [Adobe Design Principles](https://www.adobe.com/express/learn/blog/8-basic-design-principles-to-help-you-create-better-graphics) / [Adobe Design Blog](https://www.adobe.com/express/learn/blog/tags/design)
9. [UX Laws](https://cdn2.hubspot.net/hubfs/2799924/Infographics/Infographic-The-Laws-of-UX-Toptal.pdf)
10.

### Visuals

**_Developing in PowerBI_**

1. [Developing Visuals](https://learn.microsoft.com/en-us/power-bi/create-reports/)
2. [Charticulator](https://charticulator.com/docs/user-interaction.html#data-driven-guides)
3. [Deneb](https://deneb-viz.github.io/simple-example) / [AppSource](https://appsource.microsoft.com/en-us/product/PowerBIVisuals/coacervolimited1596856650797.deneb?exp=kyyw)
   - [Vega](https://vega.github.io/vega/) /
   - [Blog](https://kerrykolosko.com/exploring-deneb-for-power-bi/)

**_SVG for Visuals_**

1. [Super Charge your visuals with in Power BI with svg](https://medium.com/microsoft-power-bi/supercharge-your-data-visualizations-with-svgs-in-power-bi-4df3b89bec85)
2. [Hat Full of Data](https://hatfullofdata.blog/svg-in-power-bi-part-1/)
3. [Bing](https://www.bing.com/search?q=using+svg+in+power+bi&qs=SC&pq=using+svg+in+powerbi&sc=10-20&cvid=7572CFA1111545FBA6D409DB4C158A01&sp=1&lq=0&first=11&FORM=PERE)

**_also nuttig_**

1. [Empty character](https://emptycharacter.com/)
2. [Unicodes](https://symbl.cc/en/)
3. [Flags](https://flagpedia.net/download/api) / [flags 2](https://github.com/risan/country-flag-emoji-json)
4. [SVG repo](https://www.svgrepo.com/collections/filled/)
5. [PureViz / Powerpoint als Visual ontwerper](https://pureviz.net/infographic)

**_PowerQuery_**

[MS Learn](https://learn.microsoft.com/en-us/power-query/power-query-what-is-power-query)

**_Parameterize PowerQuery_**

1. [Power Query Snippets](C:\Users\bert.dekker\Documents\Notes\Snippets\M)
2. ![Parameterize PowerQuery](Pics/230411-125354.png)

**_External Tools for PowerBI_**

1. [Analysis Services Tools](https://learn.microsoft.com/en-us/analysis-services/tools-and-applications-used-in-analysis-services?view=asallproducts-allversions)
2. [Tabular Editor](https://tabulareditor.github.io/)
3. [DAX studio](https://daxstudio.org/docs/intro/) /
4. Bravo
5. [ALM Toolkit](http://alm-toolkit.com/)
6. VertiPac Analyser

## Tips and Trics

### highlighting the min and max value in a matrix

1. [SQLBI](https://www.sqlbi.com/articles/highlighting-the-minimum-and-maximum-values-in-a-power-bi-matrix/)
