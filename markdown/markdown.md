### Markdown notes

```
Three backticks (```) will create a block
```
<hr />

# \# Heading 1

## \## Heading 2

##### \##### Heading 5

###### \###### Heading 6

<hr />


\*\***bold**\*\*    

\**italic*\*

\~~ ~~strikethrough~~ \~~    

\*\*\****bold+italic***\*\*\*    

<hr />

Checklist in markdown

```
- [ ] item 1
- [x] item 2
- [x] item 3
```

- [ ] item 1
- [x] item 2
- [x] item 3




<hr />

Link example

``` [Duck Duck Go](https://duckduckgo.com) ```

[Duck Duck Go](https://duckduckgo.com)


To go to a section on the same page:
``` [text](#anchortext) ```

To go to a section on another page.
``` [text](filename.md#anchortext) ```


----------------------------------------------

Create links within the markdown document.  Ensure that the path replaces all spaces with a hyphen/dash as seen below.

```
[1. Lab - Main section](#lab-1---main-section)
- [1.1. Exercise - Exercise 1](#exercise---exercise-1)
- [1.2. Exercise - Exercise 2](#exercise---exercise-2)

## Lab 1 - Main Section
## Exercise - Exercise 1
## Exercise - Exercise 2
```


[1. Lab - Main section](#lab-1---main-section)
- [1.1. Exercise - Exercise 1](#exercise---exercise-1)
- [1.2. Exercise - Exercise 2](#exercise---exercise-2)


## Lab 1 - Main Section
## Exercise - Exercise 1
## Exercise - Exercise 2


<hr />
 
\!\[image name\]\(\/images\/test.png\)


![image name](../images/test.png)

<hr />

* asterisk used for bullets
+ plus used for bullets
- minus used for bullets


\<hr /> used for separation line
<hr />


Use  \`\`\`diff to show lines that are added and subtracted from the code block using  \+  and  \-  

```diff
connect-azAccount

$context = Get-AzSubscription -SubscriptionId [xxxxxxxx]
- Set-AzContext
+ Set-AzContext $context

get-azContext
```


```
```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
```
Creates the code block below:
```

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

```
\| Column 1 \| Column 2 \| Column 3 \|   
\| :------ \| :------: \| -----: \|   
\| A1 \| A2 \| A3 \|   
\| B1 \| B2 \| B3 \|   
```

Creates the table below:  

| Column 1 | Column 2 | Column 3 |   
| :------ | :------: | -----: |   
| A1 | A2 | A3 |   
| B1 | B2 | B3 |   


Colons provide left and right text justification.   


```
Markdown treats these characters as ordinary text if there is backslash escape character in front of them:   
\\ backslash itself   
\` backtick   
\* asterisk  
\_ underscore   
\{ \} curly braces   
\[ \] square brackets   
\( \) parentheses   
\# hash mark   
\+ plus sign   
\- minus sign (hyphen)   
\. dot    
\! exclamation mark    
```   
