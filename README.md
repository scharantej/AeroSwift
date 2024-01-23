## **Flask Application Design for Autonomous Helicopter**

### **HTML Files:**

- **index.html**: This will be the homepage of the application, providing an interface for the user to interact with the application.
  - Includes a form with fields for specifying the helicopter's desired flight path and other parameters.
  - Has buttons for submitting the form, displaying the status of the helicopter, and initiating its flight.


- **status.html**: This page will display the real-time status of the helicopter, including its current position, altitude, and any potential issues.


- **mission_complete.html**: This page will be displayed once the helicopter successfully completes its mission. It will show a confirmation message and any relevant details about the mission.


### **Routes:**

- **@app.route('/'**): This route will handle the homepage, serving the `index.html` file.


- **@app.route('/submit_flight_path'**, methods=['POST']): This route will process the flight path data submitted by the user, initiating the autonomous helicopter's mission.


- **@app.route('/get_status'**): This route will handle requests for the helicopter's current status, returning the relevant information in a JSON format.


- **@app.route('/mission_complete'**): This route will be called when the helicopter successfully completes its mission, displaying the `mission_complete.html` page.