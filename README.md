# Smart Classroom & Timetable Scheduler
A fully interactive web-based system designed to help universities manage faculty, subjects, classrooms, and automatically generate optimized timetables.
This project uses HTML, Tailwind CSS, JavaScript (with jQuery), and LocalStorage to build a responsive and user-friendly interface for administrators.

## Features
## Admin Login
- Secure login modal
- Default credentials:
  - Username: admin
  - Password: lpu2025
- Credentials can be updated inside the Settings section
- Updated credentials are saved in LocalStorage

## Faculty Management
- Add, edit, and delete faculty
- Store department, email, max weekly hours, availability, preferred slots
- Data saved automatically in LocalStorage
- Real-time faculty count displayed on the dashboard

## Subject Management
- Add subjects with:
  - Code, name, credits, hours/week
  - Type (Theory/Lab/Tutorial)
  - Assigned faculty (IDs)
- Edit/delete subjects anytime
- Automatically updates dashboard stats

## Classroom Management
- Add classroom with:
  - Room ID, name, capacity
  - Room type (Theory Room, Lab, etc.)
  - Facility (Projector)
- Edit/delete classrooms
- View complete room list in a table

## Timetable Generation
- Select semester and program
- Built-in constraints:
  - Avoid room clashes
  - Prevent faculty overload
  - Avoid 3+ consecutive lectures
  - Prefer morning labs (optional)
- Generates an optimized timetable (stored in LocalStorage)
- Table view with filtering options:
  - All
  - Faculty view
  - Room view
  - Program view
 
## TimeTable Export
- Export timetable to PDF with one click

## Settings
- Update login username and password
- Auto logout after changes
- Secure validation

## Tech Stack

| Technology       | Purpose                        |
| ---------------- | ------------------------------ |
| **HTML5**        | Structure and UI               |
| **Tailwind CSS** | Styling and responsive UI      |
| **JavaScript**   | Core logic and data handling   |
| **jQuery**       | DOM manipulation and utilities |
| **LocalStorage** | Persistent data saving         |
| **Font Awesome** | Icons                          |

## How Data is Stored
This project uses LocalStorage to store:
| Key                    | Data Stored         |
| ---------------------- | ------------------- |
| `schedulerCredentials` | Username & Password |
| `schedulerFaculty`     | Faculty list        |
| `schedulerSubjects`    | Subject list        |
| `schedulerClassrooms`  | Classroom list      |
| `schedulerTimetable`   | Generated timetable |

## How to Run the Project
1. Download the project files
2. Open the index.html file in any modern browser:
   - Chrome
   - Firefox
   - Edge
3. The system loads automatically—no server setup needed

## Author
This system is created as part of a Smart Classroom management and timetable scheduling project.
Fully developed using Frontend Web Technologies with a focus on usability and academic automation.
