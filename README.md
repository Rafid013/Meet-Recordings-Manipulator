# Meet Recordings Manipulator

* This is a [Google Apps Script](https://script.google.com/home) Project for manipulating Google Meet Recording files saved in Google Drive
* Developed for personal use 
* Open the project file in [Google Apps Script](https://script.google.com/home). DriveApp and Drive Api services also has to be enabled
* Change the first few variable's values in accordance with usage requirements (follow the comments)
    * The variable course_name should be set to the name of the calendar event (name of the course)
    * The variable source_folder_id should be set to the folder id of the Meet Recordings folder (where the recordings are being saved)
    * In the variable sections_folder_id add the desired sections and the desired destination folder ids for those sections according to the format
* The naming pattern in the code is <course_name> (<section_name>) (<YYYY-MM-DD>). For example, if the course name is **CSE 2213 Discrete Mathematics**, section is **F** and date is **2021-04-09**, the filename will be changed to **CSE 2213 Discrete Mathematics (F) (2021-04-09)**
* The code is mainly written for online class recordings
* This script changes the file name (adjusts the data to the GMT+06 time zone), changes share permissions, enables download options for viewers and finally moves it to the destination folder
* The script deletes the chat history
* This script is ran automatically by Google Cloud Platform based on the added triggers


