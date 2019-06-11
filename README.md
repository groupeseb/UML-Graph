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

### includes
This folder contains _css_ stylesheet and _js_ libraries used by _index.html_.
