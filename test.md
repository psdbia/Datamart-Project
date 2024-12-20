# This Page for Project

Here is the [ULTIMATE cheatsheet](https://github.com/im-luka/markdown-cheatsheet/blob/main/README.md) for mdl.


#### Table of Contents

1. [Paragraph](#paragraph)
2. [Headings](#headings)

---
The mart will be constructed as follows:  
![ERD](./data/SampleProjectERD.png)

---
<a name="paragraph" />

## Paragraph
By writing regular text you are basically writing a paragraph.

```
This is a paragraph.
```
This is a paragraph.

---

<a name="headings" />

## Headings
There are 6 heading variants. The number of "#" symbols, followed by text, indicates the importance of the heading.

```
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

## Sample SQL
```
USE TargetMartII;
GO

/*********************************************************/
/******************    Schema DDL       ******************/
/*********************************************************/

IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = 'dim' ) 
BEGIN
	EXEC sp_executesql N'CREATE SCHEMA dim AUTHORIZATION dbo;'
END
;

GO

IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = 'stg' ) 
BEGIN
	EXEC sp_executesql N'CREATE SCHEMA stg AUTHORIZATION dbo;'
END
;

GO

IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = 'f' ) 
BEGIN
	EXEC sp_executesql N'CREATE SCHEMA f AUTHORIZATION dbo;'
END
;

GO
```
