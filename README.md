# Vehicle Management System

## Overview
This Vehicle Management System captures vehicle number plates using image recognition, logs the entry and exit times, and calculates the duration of stay within the campus. The system displays the vehicle data on a React.js table view for easy monitoring and management.

## Features
- **Number Plate Recognition:** Captures and saves number plate images using a camera.
- **Data Logging:** Stores entry and exit times along with number plate data in a JSON file.
- **Duration Calculation:** Automatically calculates the time spent on the campus.
- **Real-time Monitoring:** Displays vehicle details using a React.js table view.

## Components
1. **Backend:** Python (FastAPI) for image processing, data storage, and API endpoints.
2. **Frontend:** React.js for displaying vehicle data in a table format.
3. **Database:** JSON file for storing vehicle information.
4. **Image Processing:** OpenCV or similar library for number plate recognition.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo/vehicle-management-system.git
    cd vehicle-management-system
    ```

2. Install backend dependencies:
    ```bash
    cd backend
    pip install -r requirements.txt
    ```

3. Install frontend dependencies:
    ```bash
    cd frontend
    npm install
    ```

## Usage

1. Start the backend server:
    ```bash
    cd backend
    uvicorn main:app --reload
    ```

2. Start the frontend server:
    ```bash
    cd frontend
    npm start
    ```

3. Access the system at `http://localhost:3000`

## API Endpoints
- **POST /entry** - Capture number plate image and store data
- **POST /exit** - Log exit time and calculate duration
- **GET /vehicles** - Fetch all vehicle data

## Example Data (JSON)
```json
[
  {
    "S.No": 1,
    "Number Plate Image": "images/image1.jpg",
    "Vehicle Number": "TN93E****",
    "Date": "29-11-2024",
    "Time": "09:18:21",
    "Status": "Entry"
  }
]
```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License.

## Contact
For questions or suggestions, feel free to contact.
