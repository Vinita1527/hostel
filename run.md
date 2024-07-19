# Hospitality Process Digitalization

## Overview

This web application facilitates the digitalization of the hospitality process for group accommodation. It allows users to upload CSV files containing group and hostel information, process these files to allocate rooms, and download the results as a CSV file.

## Features

- **File Upload**:
  - Upload two CSV files:
    - **Group Information CSV**: Contains details about the groups needing accommodation.
    - **Hostel Information CSV**: Contains details about available hostels and their rooms.

- **Room Allocation**:
  - The system processes the uploaded files to allocate rooms based on gender and capacity constraints.

- **Result Display**:
  - Shows the room allocation results in a table format on the web page.

- **CSV Download**:
  - Provides an option to download the allocation results as a CSV file.

## Instructions to Run the Application

1. **Save the HTML File**:
   - Save the code provided as `index.html`.

2. **Open in Browser**:
   - Open the `index.html` file in your preferred web browser.

3. **Upload Files**:
   - **Group Information CSV**:
     - Click on the "Choose File" button under "Upload Group Information CSV".
     - Select the CSV file containing group information. Ensure the file contains columns: `Group ID`, `Members`, and `Gender`.
   - **Hostel Information CSV**:
     - Click on the "Choose File" button under "Upload Hostel Information CSV".
     - Select the CSV file containing hostel information. Ensure the file contains columns: `Hostel Name`, `Room Number`, `Capacity`, and `Gender`.

4. **Process Files**:
   - Click "Process and Allocate Rooms" to process the files and allocate rooms.

5. **View and Download Results**:
   - View the results in the table displayed on the page.
   - Click "Download CSV" to download the results as a CSV file.

## Technical Details

- **HTML Structure**: Used for uploading CSV files and displaying results.
- **CSS Styling**: Features a gradient background for a modern look, with a styled container and enhanced table and button styles.
- **JavaScript Functionality**:
  - **File Reading**: Uses FileReader and PapaParse to read and parse CSV data.
  - **Room Allocation Logic**: Allocates rooms based on group size and room capacity, and updates room capacities accordingly.
  - **CSV Download**: Converts the results table to CSV format and triggers a download.

## Future Enhancements

- **Improved Error Handling**: Display user-friendly error messages for common issues.
- **Enhanced Data Validation**: Ensure that CSV files have valid and complete data before processing.
- **User Interface Improvements**: Add more styling options and interactivity for a better user experience.

This `README.md` file provides a comprehensive overview of the application, including its features, usage instructions, technical details, and future enhancement plans.
