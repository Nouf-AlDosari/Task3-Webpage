 📋 Project Description:
This project is a web-based control panel for a robot arm consisting of 6 motors. The interface allows you to adjust motor positions using sliders, save poses to a MySQL database, load poses, run the last saved pose, and delete them.

---
 🧰 Requirements:
- PHP Server (e.g., XAMPP or WAMP)
- MySQL Database
- Web Browser
- Text Editor (e.g., Visual Studio Code)
---
📁 Project Contents:
- index.html: The main UI with motor sliders.
- save_pose.php: Saves motor values to the database.
- load_table.php: Loads the saved poses table.
- load_pose.php: Loads a specific pose by ID.
- delete_pose.php: Deletes a pose.
- get_run_pose.php: Retrieves the most recent pose with status = 1.
- update_status.php: Sets all poses' status to 0.
- robot_arm_table_preview.jpg: Example image of pose table.
- database.sql: SQL file to create the necessary database and table.
---
 🧱 Database Setup:

1. Open phpMyAdmin.
2. Create a database named robot_arm.
3. Run the SQL code from database.sql.
CREATE DATABASE robot_arm;
USE robot_arm;

CREATE TABLE poses (
    id INT AUTO_INCREMENT PRIMARY KEY,
    motor1 INT,
    motor2 INT,
    motor3 INT,
    motor4 INT,
    motor5 INT,
    motor6 INT,
    status INT DEFAULT 0
);

---
🚀 How to Run:

1. Place all files inside your local server directory (e.g., htdocs in XAMPP).
2. Open your browser and go to:  
   http://localhost/robot_arm_project/index.html
3. Use the sliders to adjust the 6 motor positions.
4. Click:
   - Save Pose to store the current position.
   - Run to run the most recently saved pose.
   - Reset to return all values to 90.
   - Load/Remove to work with saved poses from the table.
---
 ✅ Additional Features:
- get_run_pose.php: Returns the latest pose with status=1.
- update_status.php: Resets all statuses to 0 (useful after running).
---
 📸 Pose Table Preview:
An image (`robot_arm_table_preview.jpg`) is included in the project folder to preview how the table will look.
![Image](https://github.com/user-attachments/assets/8080df7e-5fac-41c1-9fca-1efea2243097)

---

<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/dc1967ef-60bb-4711-af14-b6c01fd791cb" />


