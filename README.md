# DigitalTwin
This is a project where I am experimenting with Digital Twin Technology.

## Personal Research
### Digital Twin background
- A Digital Twin of any device/system is a working model of all components integrated and mapped together using physical data, virtual data, and interaction between them to make a fully functional replica of the device/system and that too on a digital medium. - geeksforgeeks.org
- They are typically used to represent large scale machines or factories.
- My version is just the 3D representation part of the typical package.

### Data available
- Possible data suppliers for AUV:
    - Sonar (2D Map of surroundings)
    - IMU (Accelerometer / Gyroscope / Magenetometer)
    - Voltage / Current Measurements (Voltage and Amperage)
    - Hydrophone heading direction (Compass directions)
    - Leak Detection
    - Depth Sensor (meters)
    - Internal Temperature
    - External Temperature
    - Internal Humidity
    - Internal Pressure
    - External Pressure
    - ZED 3D maps of perspective view point

### When data will be supplied
- This won't be real-time since the host machine is located at the lab
- During run the data will be stored locally and when internet is available it will be uploaded to the remote server
- When data is uploaded, the model will analyze the uploaded data and represent it as a historical record (Think video scrubbing)

### Environment
- Create docker-compose and dockerfile to containerize the app
- Using `three.js` for the 3D environment and data vizualization
- Using `electron.js` to create the application and handle the database connection

## What I would like to accomplish for this project:
1. Create a docker runtime to containerize the app and run on the server in the lab
2. Display a 3D representation of the sub with data views (graphs, charts, tables)
3. Display the none 3D representable data in tables and charts
4. Project the Sonar and ZED data as viewable data within the 3D representation (ie. the environment around the sub represented)

## References:
1. https://www.geeksforgeeks.org/introduction-to-digital-twin/
2. https://www.electronjs.org/docs/latest/tutorial/tutorial-first-app
3. 