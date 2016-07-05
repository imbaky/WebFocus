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

<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/1999/REC-html401-19991224/strict.dtd">
<html>
<head>
<META http-equiv=Content-Type content="text/html; charset=UTF-8">
<title>Exported from Notepad++</title>
<style type="text/css">
span {
	font-family: 'Courier New';
	font-size: 10pt;
	color: #000000;
}
.sc0 {
}
.sc2 {
	color: #008000;
}
.sc4 {
	color: #FF0000;
}
.sc24 {
}
</style>
</head>
<body>
<div style="float: left; white-space: pre; line-height: 1; background: #FFFFFF; "><span class="sc2">-* COMMMENT 
</span><span class="sc24">
</span><span class="sc0">[</span><span class="sc24"> </span><span class="sc4">TABLE</span><span class="sc24"> </span><span class="sc0">|</span><span class="sc24"> </span><span class="sc4">GRAPH</span><span class="sc24"> </span><span class="sc0">]</span><span class="sc24"> </span><span class="sc4">FILE</span><span class="sc24"> </span><span class="sc0">[Data</span><span class="sc24"> </span><span class="sc0">source]</span><span class="sc24">
</span><span class="sc0">[</span><span class="sc24"> </span><span class="sc4">PRINT</span><span class="sc24"> </span><span class="sc0">|</span><span class="sc24"> </span><span class="sc4">SUM</span><span class="sc24"> </span><span class="sc0">]</span><span class="sc24">
</span><span class="sc0">[Data</span><span class="sc24"> </span><span class="sc0">Columns]</span><span class="sc24">
</span><span class="sc0">[Sort</span><span class="sc24"> </span><span class="sc0">Type]</span><span class="sc24">
</span><span class="sc0">[Filter</span><span class="sc24"> </span><span class="sc0">Definition]</span><span class="sc24">
</span><span class="sc0">[Output</span><span class="sc24"> </span><span class="sc0">Definition]</span><span class="sc24">
</span><span class="sc0">[Style</span><span class="sc24">  </span><span class="sc0">Definition]</span><span class="sc24">
</span><span class="sc0">END</span></div></body>
</html>



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
## Tips and Tricks
