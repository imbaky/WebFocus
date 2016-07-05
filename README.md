# WebFocus

## Introduction
Webfocus is really powerful and useful tool but it takes a while to get used to, I personally struggled as a Co-op student to grasp it but once you get it, it becomes alot simplier. That's why I've decided to write this to help others learn and understand it. 

If you are still new to webfocus, you will soon realize that using the gui (DevStudio, AppStudio..wtv) restricts you in alot of different ways and might even discourage you from using it so what I would suggest is that you learn to write Focus code yourself first then you can explore the gui and actually understand what it can and can not do.

##Terms
* Report
* Procedure 
* Graph
* Synonyms



##Types of files 
1. '*.FEX' : 
2. '*.MAS' : A Master File describes a data source using a series of declarations(Metadata)
3. '*.ACX' :
4. '*.FTM' : The raw data file with the resultset of the query.

##Syntax and Structure

```
-* COMMMENT 

[TABLE|GRAPH] FILE [Data source]
[PRINT|SUM]
[Data Columns]
[Sort Type]
[Filter Definition]
[Output Definition]
[Style  Definition]
END
```



### Data Source
* Synonyms

### Data Columns

* Max.[Column_Name]
* MIN.[Column_Name]
* AVE.[Column_Name]
* SUM.[Column_Name]

### Sort Type
* BY
* ACROSS
* SUBHEAD

### Filter Definition
```
WHERE [Column] [Qualifier] [Value] ;
```
Qualifiers: 
* 'EQ': Equal
* 'LT': Less Then
* 'GT': Greater Then
* 'GE': Greater then or Equal
* 'NE': Not Equal
* 'BETWEEN' [value_1] and [value_2] 
* 'IN LIST' [List of values]: Checks if value is in the list of values provided

### Output Definition
You can either output a file with your result as shown below:

```
ON TABLE PCHOLD FORMAT [Output Format]
```
Or you can hold the results for later use like this:
```
ON TABLE HOLD AS [Hold_Name] FORMAT [Output Format]
```

Output Formats:
* HTML
* PDF
* EXL2K
* WP
* ALPHA
* XML
* FOCUS

### Style  Definition
```
ON TABLE SET STYLESHEET *
TYPE=type, [COLUMN=column_name],
property=value,[property=value,]...$
[TYPE=type, [COLUMN=column_name],
property=value,[property=value,]...$
[TYPE=type, [COLUMN=column_name],
property=value, [property=value,]...$]…
ENDSTYLE
```
### Charts
### Debugging Techniques
## Tips and Tricks
