# 🧩 HTML Syntax Checker using Pushdown Automata (PDA)

## Project Overview
Welcome to the HTML Syntax Checker using Pushdown Automata (PDA) project! This repository represents my third-semester assignment for the Formal Language and Automata Theory course at ITB.

## General Information
HTML (Hypertext Markup Language) serves as a markup language utilized in shaping the structure and visual presentation of web content. Through elements (tags), HTML organizes and groups content. Similar to most languages, HTML maintains its own syntax for writing, the violation of which can lead to errors. An error detection program for HTML is essential to verify the accuracy of tag usage and its associated attributes.

## Technologies Used
- Python3

## Features

Considering many types of tags and attributes available in HTML, the scope of programming assignments will be limited. The limitations of the tags and attributes checked can be seen below.
| Tag | Attributes | Void Element | Notes |
|---|---|---|---|
|html| | |The html tag is mandatory. The document must begin with the html tag|
|head| | |A head tag must be present. The head tag must be inside the html tag and above the body tag|
|body| | |The body tag must be present. The body tag must be inside the html tag and below the head tag. All elements mentioned after this except the title must be in the body, but not all tags must be in the body.|
|title| | |can only be in the head|
|link| Rel, href | V |The Rel attribute must be present, it can be in the head|
|h1, h2, h3, h4, h5, h6| | | |
|p| | | |
|br| | V | |
|em| | | |
|b| | | |
|abbr| | | |
|strong| | | |
|small| | | |
|hr| |V| |
|div| | | |
|a|href| | |
|img| src, alt | V | src attributes is mandatory |
|button| type |  | The attribute type value is limited to submit, reset, button |
|form| action, method |  | The method value must be limited to GET or POST |
|input| type | V | The attribute type value must be limited to text, password, email, number, or checkbox |
|table| | | You don't need to pay attention to the shape of the table (it's okay if row 1 consists of 1 column while row 2 consists of 2 columns) |
|tr| | |The tr tag must be in the tag table|
|td| | |The td tag must be in the tag table|
|th| | |The th tag must be in the tag table|
###
This program also has an additional feature, namely telling you where the error in the HTML code entered. The program can also explain what expressions are wrong in the program, such as inappropriate use of tags or attributes. The program can also detect errors involving the HTML program code structure.

## Structure
```
├── readme.md
│ 
├── doc
│   └── .pdf
│       
├── pda
│   ├── pda.drawio
│   └── pda.png
│ 
└── src
    ├── main.py
    │ 
    ├── functions
    │   ├── load.py
    │   └── readpda.py
    │
    ├── html
    │   ├── input.html
    │   ├── inputAcc.html
    │   ├── inputReject.html
    │   └── testing.html
    │
    └── pda
        ├── pda txt guide.md
        ├── pda.drawio
        ├── pda.png
        └── pda.txt
```
---

## How to Use
    git clone https://github.com/rizqikapratamaa/HTML-Syntax-checker-using-Pushdown-Automata
    cd HTML-Syntax-checker-using-Pushdown-Automata/src
    python main.py pda.txt <test-case-name>.html

### Dependencies
- Python Interpreter

### Installation
- Download and install [Python](https://www.python.org/downloads/)
- Download all folder and files on this repository or simply clone this repo!