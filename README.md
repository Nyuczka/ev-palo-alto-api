# ev-palo-alto-api

Simple project for connection between Flask and Spring Boot API's. 
Data used are the information about charging station events in Palo Alto. 
This project is not finished. The final version will be uploaded later. 
For more information, please check TO-DO section. 

## Requirements
In order to run this project, you need to have MYSQL 8, Python 3.9, Java 11, Pip and Maven 3 installed. 
Here are the links for Installation Packages/Guides: 
- [MYSQL Download](https://dev.mysql.com/downloads/mysql)
- [Python Download](https://www.python.org/downloads)
- [Java 11 Download](https://www.openlogic.com/openjdk-downloads)
- [Pip Installation](https://pip.pypa.io/en/stable/installation/)
- [Maven 3 Installation](https://maven.apache.org/install.html)

## Setup 
1. Run MYSQL instance on your local machine.
2. Clone the project using `git clone https://github.com/Nyuczka/ev-palo-alto-api.git`.
3. Open terminal and to `station-entry-api` folder.
4. Run `mvn clean install` command.
5. In new terminal tab go to `charging-station-api` folder. 
6. Run `pip install requirements.txt` command. 

## Running the project
1. Go to `station-entry-api` and run `mvn spring-boot:run` command from terminal. This API will run on `8080` port.
2. Go to `charging-station-api` and run `python3 app.py` command from terminal. This API will run on `5000` port.
3. Open Postman and import `EV-charging-station-requests.postman_collection.json` for testing.


## TO-DO:
### station-entry-api
1. Update post mapping for adding new entry. 
2. Update code for accepting admin user for add-entry call. 
3. Create unit tests. 

### charging-events-api
1. Add caching.
2. Update post mapping for adding new entry.
3. Create unit tests.

### ev-palo-alto-api
1. Add docker-compose file. 
2. Update the README for docker-compose setup. 
