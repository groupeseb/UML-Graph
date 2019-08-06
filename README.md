# UML Graph
This project aims to provide some little tools to manage and visualize Camel Routes from OFS-Bus project.

## Main files

### index.html
This html page allows to visualize Camel Routes' information stored in _routes.csv_ file.
Mainly, it has javascript code based on _d3_ and _jquery_ libraries.

### routes.csv
This CSV file contains detailed information of the status of any Camel Route and the routes that are called by them.
For further information you can read [this documentation](https://confluence.seb.com/display/DW/Camel+Audit).

### xmi2csv.html
This file merely contains a script to transform a XMI file to a CSV. It was used to transform generated XMI file by
[Modelio](https://www.modelio.org/) tool to an easier to handle format.  
Early on Camel Audit task, we used Modelio to draw manually an UML graph of all Camel Routes. It was a hard work and
the graph became unreadable. So, we decided to export the current work and find another solution.

### machine-state-diagram.xmi
This is the generated file by Modelio.

## resources-by-domain.xlsx
List of all existing resources grouped by domain.

### includes
This folder contains _css_ stylesheet and _js_ libraries used by _index.html_.

## How to run
Modern browsers blocks CORS requests. In this case, _index.html_ is not allowed to load _routes.csv_ file.  
To avoid that, we can run a local server to retrieve our local files.

* Install **node.js** http-server: `npm install http-server -g`
* Go to project root folder.
* Run the server on folder _src_: `http-server ./src`

By default this server uses port 8080. Anyway, pay attention to the information showed when start.  
Now, we can access to _index.html_ by the URL http://localhost:8080/index.html

For further information see https://www.npmjs.com/package/http-server
