# WebFocus

## Introduction
Webfocus is really powerful and useful tool...if you know how to overcome its issues, which took me a while to figure out as a coop student. So I've decided to write this to help others learn and excel in using Webfocus effeciently.

If you are still new to webfocus, you will soon realize that using the gui (DevStudio, AppStudio..wtv) restricts you in alot of ways and might even discourage you from using Webfocus so what I would suggest is that you learn to write focus code yourself first then you can explore the gui and actually understand what it can and can not do.

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

```FOCUS
-* COMMMENT 

[TABLE|GRAPH] FILE [Data source]
[Print Type]
[Sort Type]
[Filter Definition]
[Output Definition]
[Style  Definition]
END

```


### Data Source
* Synonyms

### Print Type
* PRINT
* SUM

### Sort Type
* BY
* ACROSS
* SUBHEAD

### Filter Definition
* WHERE

### Output Definition
```
ON TABLE PCHOLD FORMAT [Output Format]
```
#### Output Formats
* HTML
* PDF
* EXL2K
* 

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
