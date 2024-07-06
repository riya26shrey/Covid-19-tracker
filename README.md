# Coronavirus - Covid 19 tracker
The idea behind this application is to display global statistics for Coronavirus COVID-19, constantly updating the case data sourced from a reliable data repository.

## Technical Overview
This full-stack application utilizes React.js for the front-end and Node.js for the back-end. It retrieves and parses COVID-19 data from a data repository and stores it in MongoDB.

The application utilizes Mapbox to visualize geographical data using GeoJSON format.

<img src="Screenshots/covid19.png"/>

### MongoDB Sample Database Import Command
After cloning the repository, import sample statistics into your local MongoDB database to kickstart the project.

```
git clone https://github.com/riya26shrey/Covid-19-tracker.git
cd covid 19 tracker

mongod (Start MongoDB database)

mongoimport --uri "mongodb://127.0.0.1:27017/covid-19" --collection covid_statistics --file dummy_statistics.json
```

### Server Installation
```
cd server
npm install
npm start
```
Open [http://localhost:9000](http://localhost:9000) in your browser.

### Client Installation
```
cd client
npm install
npm start
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Changing Constants in Client App
Update the following constants in your client application:

```javascript
export const BASE_URL = `http://YOUR_LOCAL_IP_ADDRESS:9000`;
export const MAPBOX_ACCESS_TOKEN = `YOUR_MAPBOX_API_TOKEN`;
```

### MAPBOX Styles
The following Mapbox styles are used in the application:

```
mapbox://styles/hackbotone/ck8vtayrp0x5f1io3sakcmpnv
mapbox://styles/hackbotone/ck8vt8vdj2fz91ilax6nwtins
```

### Note
If you encounter any issues or have suggestions for improvement, please feel free to raise an issue.

### License
This project is licensed under the [MIT License](LICENSE)


