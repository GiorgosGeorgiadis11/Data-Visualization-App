This project aims to develop a data visualization application based on data provided by the [World Bank](http://data.worldbank.org/). More specifically, we have collected data from 25 European countries and created a UI that provides the user with various options. Based on the user's choices, we also generate the corresponding charts.

### Project Implementation:
- Spring Boot (backend)
- Html, CSS, JavaScript, Bootstrap (frontend)
- Thymeleaf (for connecting frontend with backend)
- HighCharts (graphs)

### Explanation of Folders and Files:
In the **Load data script** folder, the following files are included:
- **CountrieData**: A folder containing data for each country separately.
- **ReadyForLoad**: A folder created after running the script (`readyForLoadCsv.py`) and containing data ready to be loaded into the database.
- **globals.py**: Contains some global variables and is called in all other scripts.
- **readyForLoadCsv.py**: A script that transforms the data from the CountriesData folder and prepares it to be loaded directly into the database.
- **loadData.py**: A script that creates the database, tables, and loads the csv files, located in the ReadyForLoad folder, directly into the database.
- **main.py**: A script that runs the above 2 scripts.

In the **project** folder, all the files needed by Spring Boot to run the project are included. (the implemented code is located within the src folder)

In the **deliverables** folder, the following items are included:
- A PDF containing the project report.

### To run the project, the username and password of the database must be changed in the "Load data script/loadData.py" file and in the "project/src/main/resources/application.properties" file.

