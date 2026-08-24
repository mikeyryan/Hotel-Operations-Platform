# Product Requirements Document
## 1. Project Overview
The Hotel Operations Platform is a cross-platform application designed to improve communication between hotel staff and managers.

The system will allow staff to quickly submit service requests, document issues with photographs, and communicate those requests to hotel management.

Managers will be able to view, assign, track, and analyze service requests through a centralized dashboard.

The long-term goal is to incorporate AI to provide useful operational insights based on the data collected by the platform.

---
## 2. Problem
Hotel staff may currently communicate service requests through different methods across different platforms, which also include verbal communications, paper forms, messaging applications, or other manual processes.

This can make it difficult for managers to:

- Track requests
- Determine which requests are unresolved
- Assign tasks efficiently
- Understand staff workload
- Identify recurring problems
- Analyze hotel operations

This project aims to create one centralized system where staff users would use it more conveniently for these tasks. 

---
## 3. Primary Users
### Hotel Staff
Staff members need a convenient and simple way to: 
- Create service requests
- Document problems
- Take photographs
- Identify rooms and locations
- View assigned tasks
- Update task status

### Hotel Managers
Managers need to:
- View all requests
- Search and filter requests
- Review photoraphs
- Assign tasks
- Monitor completion
- Analyze operational activity
- Generate reports

---
# 4. MVP Features
## Staff Applications
### Authentication
- [ ] Staff login
- [ ] Secure authentication
- [ ] Staff profile
### Service Requests
- [ ] Create request
- [ ] Select category
- [ ] Select room/location
- [ ] Add description
- [ ] take photo inside application
- [ ] Preview photo
- [ ] Retake photo
- [ ] Submit request
### Task management
- [ ] View assigned tasks
- [ ] View task details
- [ ] Change task status
- [ ] Mark task as completed

---
## Manager Dashboard
### Request Management
- [ ] View all requests
- [ ] View request details
- [ ] View attached photographs
- [ ] Search requests
- [ ] Filter requests
- [ ] Sort requests

### Assignment
- [ ] View available staff
- [ ] Assign request to staff member
- [ ] Reassign request
- [ ] Monitor task status

### Analytics
- [ ] Total requests
- [ ] Open requests
- [ ] Completed requests
- [ ] Average response time
- [ ] Average completion time
- [ ] Requests by department
- [ ] Requests by category

---
# 5. ⏳ AI Features
AI features will be introduced after the core application is working...
## AI Categorization
The AI should be able to analyze a request and recommend:
- Department
- Category
- Priority
Example:
Input:
"Room 314's guests need extra water."
Possible output:
- Department: Supplies
- Category: Demanding Supplies
- Priority: Low
AI recommendations should be reviewable by managers

---
## AI Operational Analysis
The system should eventually identity:
- Recurring problems
- Department workload
- Request trends
- Unusual increases in requests
- Response-time patterns
- Potential operational bottlenecks

---
## AI Summaries
The system should eventually provide managers with summaries such as: 
"Maintenance requests increased this week, with water requests made by guests representing a significant portion of reported requests."

---
# 6. Employee Activity Metrics
The system may provide operational metrics such as: 
- Tasks completed
- Tasks completed on time
- Average response time
- Average completion time
- Number of requests handled
- Documentation quality
These metrics are intended to provide managers with information about operations.
