---
toc: true
comments: false
layout: post
title: Table full of terms
description: This post covers my plans for week 2
type: hacks
courses: { compsci: {week: 3} }
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Table Search</title>
    <style>
        /* Add some basic CSS for styling */
        table {
            border-collapse: collapse;
            width: 100%;
        }

        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }

        tr:nth-child(even) {
            background-color: #f2f2f2;
        }

        input[type="text"] {
            width: 100%;
            padding: 5px;
            margin-bottom: 10px;
        }
    </style>
<table id="myTable">

<body>
    <h2>Table Search</h2>
    <input type="text" id="searchInput" placeholder="Search for a term...">
    <br>
    
    <tr>
        <th>Commands</th>
        <th>Definition</th>
        <th>Week Learnt</th>
    </tr>
    <tr>
        <td>make</td>
        <td>This runs a local server</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>make convert</td>
        <td>Converts Jupyter Notebook files, run this if your .ipynb files are not updating on the server.</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>wsl</td>
        <td>Lets you run a Linux environment on your machine</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>cd ~</td>
        <td>Lets you change your directory to the home directory</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>cd -vscode</td>
        <td>Lets you change your directory to the VS Code directory</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>ls</td>
        <td>Checks all the files in the directory</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>code &lt;repository name&gt;</td>
        <td>Opens a repository</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>git clone &lt;link&gt;</td>
        <td>Clones a repository</td>
        <td>Learnt in Week 0</td>
    </tr>
    <tr>
        <td>print()</td>
        <td>Prints a statement</td>
        <td>Learnt in Week 1</td>
    </tr>
    <tr>
        <td>msg = input(“abcd”)</td>
        <td>When the variable `msg` is printed, the input box displays “abcd,” prompting the user to type something in the box</td>
        <td>Learnt in Week 1</td>
    </tr>
    <tr>
        <td>if expression</td>
        <td>Evaluates for true and false</td>
        <td>Learnt in Week 1</td>
    </tr>
    <tr>
        <td>#</td>
        <td>Comments out code and makes it invalid from running</td>
        <td>Learnt in Week 1</td>
    </tr>
    <tr>
        <td>lists</td>
        <td>A list is an ordered, changeable, collection</td>
        <td>Learnt in Week 2</td>
    </tr>
    <tr>  
        <td>Int</td>
        <td>The integer number type(integer numbers)</td>
        <td>Learnt in Week 2</td>
    </tr>
    <tr>
        <td>Float</td>
        <td>The floating number type(numbers with decimals)</td>
        <td>Learnt in Week 2</td>
    </tr>
    <tr>
        <td>Dictionary</td>
        <td>A dictionary is an unordered, and changeable, collection</td>
        <td>Learnt in Week 2
    </tr>
    <tr>
        <td>def(abcd)</td>
        <td>creates the function "abcd"</td>
        <td>Learnt in Week 2</td>
    </tr>
     <tr>
    <td>import</td>
    <td>imports a file into the terminal, there are multiple types of files</td>
    <td>Learnt in Week 3</td>
  </tr>
  <tr>
    <td>for loop</td>
    <td>A control flow statement used to iterate over a sequence (like a list, tuple, or string) multiple times.</td>
    <td>Learnt in Week 3</td>
  </tr>
  <tr>
    <td>while loop</td>
    <td>A control flow statement that iterates through a sequence, until a certain condition is met.</td>
    <td>Learnt in Week 3</td>
  </tr>
  <tr>
    <td>Boolean</td>
    <td>Checks for true or false</td>
    <td>Learnt in Week 3</td>

 <script>
        // JavaScript to filter the table based on the search input
        document.getElementById("searchInput").addEventListener("keyup", function() {
            const input = this.value.toLowerCase();
            const table = document.getElementById("myTable");
            const rows = table.getElementsByTagName("tr");

            for (let i = 1; i < rows.length; i++) {
                const name = rows[i].getElementsByTagName("td")[0].textContent.toLowerCase();
                if (name.includes(input)) {
                    rows[i].style.display = "";
                } else {
                    rows[i].style.display = "none";
                }
            }
        });
    </script>


