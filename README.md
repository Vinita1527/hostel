Hospitality Process Digitalization Documentation
Overview
This web application facilitates the digitalization of the hospitality process for group accommodation. It allows users to upload CSV files containing group and hostel information, process these files to allocate rooms, and download the results as a CSV file.

Features
File Upload:

Upload two CSV files:
Group Information CSV: Contains details about the groups needing accommodation.
Hostel Information CSV: Contains details about available hostels and their rooms.
Room Allocation:

The system processes the uploaded files to allocate rooms based on gender and capacity constraints.
Result Display:

Shows the room allocation results in a table format on the web page.
CSV Download:

Provides an option to download the allocation results as a CSV file.
Usage
1. Upload Files
Group Information CSV:

Click on the "Choose File" button under "Upload Group Information CSV".
Select the CSV file containing group information.
Ensure the file contains columns: Group ID, Members, and Gender.
Hostel Information CSV:

Click on the "Choose File" button under "Upload Hostel Information CSV".
Select the CSV file containing hostel information.
Ensure the file contains columns: Hostel Name, Room Number, Capacity, and Gender.
2. Process Files
Click on the "Process and Allocate Rooms" button.
The application will read the uploaded files and process them to allocate rooms based on group size and gender.
3. View Results
The results will be displayed in a table format, showing:
Group ID: The identifier for the group.
Hostel Name: The name of the hostel where the group is allocated.
Room Number: The number of the room allocated.
Members Allocated: The number of members assigned to the room.
4. Download Results
Click on the "Download CSV" button to download the allocation results in a CSV format.
Technical Details
HTML Structure
<input type="file">: Used for uploading CSV files.
<button>: Initiates the file processing and room allocation.
<table>: Displays the allocation results.
CSS Styling
Background: The page features a gradient background for a modern look.
Container: Centralized and styled with padding, shadow, and rounded corners.
Table and Button Styles: Enhanced for better visual appeal and usability.
JavaScript Functionality
File Reading:

Uses FileReader to read the contents of the uploaded CSV files.
Utilizes the PapaParse library to parse CSV data.
Room Allocation Logic:

Filters hostels by gender.
Allocates rooms based on group size and room capacity.
Updates room capacities accordingly.
CSV Download:

Converts the results table to CSV format and triggers a download.
Error Handling
File Read Errors: If a file fails to load, an error message will be logged to the console.
No Valid Allocations: The application assumes that all groups will be allocated rooms as per the data provided.
Future Enhancements
Improved Error Handling: Display user-friendly error messages for common issues.
Enhanced Data Validation: Ensure that CSV files have valid and complete data before processing.
User Interface Improvements: Add more styling options and interactivity for a better user experience.
