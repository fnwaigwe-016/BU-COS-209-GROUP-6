# Product Requirements Document (PRD)

**Product Name**: CAMPUS NAVIGATION SYSTEM 
**Course**: BU-COS 209   
**Team**: Group 6 (`BU-COS-209-GROUP-6`)  

## 1. Product Overview
This is a Navigation system that helps, incoming students, regular students, staff, visitors and even parents to be able to find their way around the campus easily no matter where it is.

## 2. Problem Statement & User Research
**The Problem**
From the research conducted, it was found out that some of the interviewed campus users have had some bad experience, either lateness to class, failure to locate a particular building, and so on.

### Primary Research Findings (Survey = 8 users)
To validate this problem, our team surveyed 8 campus community members across different groups (100-level fresher, returning students, postgraduate student, lecturer/staff, and a visitor/parent).

**Research Metric** 
| Research Metric | Survey Result (N = 8) | Key Takeaway |
| :--- | :--- | :--- |
| **Lateness due to navigation** | **62.5%** (5 out of 8) arrived late to a class, exam, or appointment | Poor wayfinding directly harms punctuality |
| **Current coping habit** | **75.0%** (6 out of 8) ask passersby, security, or porters first | High reliance on informal, error-prone human help |
| **Hardest locations to find** | **62.5%** (5 out of 8) struggle with indoor lecture halls/classrooms | Pinpointing a building exterior is not enough |
| **Most requested help** | **62.5%** (5 out of 8) want step-by-step landmark directions | Users prefer visual landmarks over raw coordinates |

### Real User Experiences (Survey Quotes)
 "When I got to a location and I was told that it was the wrong place. Only to be directed to another place and it still was the wrong location. I was just going in circles, and eventually the first place was actually where I was supposed to go."  
 — *Postgraduate Student (3+ years on campus)*

 "Walking to a different place and later finding out it was closer than where we went."  
 — *Returning Student (200-Level & above)*

### Why Existing Solutions Fall Short
- **Standard Map Apps (e.g., Google Maps):** As much as Google Maps sounds like a solution, it falls short because not every person in the campus community has an access to active mobile internet and also the school wifi might not also be effective everywhere.
  Secondly, the user, might not know the name of where he/she is going as to search on the Map.
- **Asking Passersby / Security:** A passerby might also not know the name of the place and also it affects your timing to your specific appointment when you keep stopping from time to time to inquire about direction.

## 3. Proposed Solution
A system where the campus community can be able to find their way easily using landmark-based walking directions, a specific search for each building on campus, and also a campus directory that is easy for even a visitor to read.

## 4. Target Users
- **New & Returning Students:** Especially 100-level freshers navigating their way through lecture and administrative halls.
- **Campus Visitors & Parents:** Those who do not know the buildings by their nicknames or the shortcuts.
- **Campus Administrators / Student Reps:** Those who maintain building records, room allocations, and gate schedule.


## 5. MVP Scope & Features

### In-Scope (Version 1 MVP)
1. **Keyword & Nickname Search:** Users can search or know a building by its nickname.
2. **Building-to-Room Directory:** Users can click on a building to see its floors and specific room directions.
3. **Landmark-Based Walking Directions:** Users can be guided using a Landmark in order to recognize a particular building.
4. **Operating Hours & Gate Status:** Users can be able to plan their time and accessibility in order to avoid delay or missed appointments.
5. **Admin Venue & Closure Management:** Management keeps the directory accurate, so users aren't sent to locked buildings or renamed buildings.


## 6. Detailed Requirements, User Stories & Acceptance Criteria

### Feature 1:  Nickname Search
- **User Story:** As a 100 level Student, I want to be able to know the lecture halls by their nickname so that i can easily find the place when i don't know it by the name written on my time table.
- **Acceptance Criteria:**
  - Type searching either the official or nickname of that building that returns to same building.
  - Text search result load quickly even with a poor internet connection.

### Feature 2: Indoor Location Data
- **User Story:** As a student looking for a classroom, I want to know the exact floor and room details so that i don't go back and forth in the wrong place.
- **Acceptance Criteria:**
  - Displays Building -> Floor -> Wing -> Room description
  - Includes entrance or landmark photos

### Feature 3: Landmark & Footpath Walking Directions
- **User Story:** As a visitor or parent, I want to be able to use visible landmarks so that i don't get lost while asking passerby.
- **Acceptance Criteria:**
  - Routes include pedestrian shortcuts.
  - Uses visible campus landmarks instead of street names alone.
    
## Functional Requirements
- **Keyword & Nickname Search**`: Users can search for any building, lecture hall, or office using either its official name or common student nicknames (e.g., New Horizon, Bucodel, SAT).
- **Room Lookup**: Selecting a building displays its internal breakdown—Building → Floor → Wing → Room description—along with reference photos of the entrance or nearby landmarks.
- **Landmark-Based Walking Directions**: Users can pick a starting point (like the Main Gate or Cafeteria) and get step-by-step walking directions that use visible landmarks and pedestrian shortcuts.

## Non-Functional Requirements
- **Performance on Low Connectivity**: Because mobile data and campus Wi-Fi can be slow in certain areas, lightweight text directions and room details must load within 2–3 seconds before heavy entrance photos are downloaded.
- **Availability During Peak Hours**: The system must remain reliable and accessible during high-traffic periods—such as 7:00 AM lecture rushes, exam weeks, and resumption/convocation days.
- **Usability for First-Time Visitors**: The search and step-by-step instructions must be simple enough for a parent or visitor to understand immediately without a guide.
- **Security & Role-Based Access**: Public users (students, staff, visitors) can search and view locations freely without logging in, while only authenticated campus administrators can add, edit, or delete venue records.

### Edge Cases Handled
- **Poor Internet Connectivity:** The system displays the text directions and room details first before the photos so the users can still navigate even with poor internet connection.
- **Duplicate Room Numbers:** Every room should display each building and faculty name (e.g. Lecture Room 1 New Horizon or Lecture Room 1 Bucodel) so that student doesn't end up in the wrong building 
- **Closed Gates After Hours:** System checks available gates and redirects the user to the available gate open.


## 7. Success Metrics
- **Active Searches:** Upon resumption, freshers, visitors and parents will be looking for offices, hostels etc. We have a target to have at least 300+ weekly searches.
- **Reduction in Lateness:** Reduce venue-related lateness from our **62.5% survey baseline** to under **20%**.
- **Self-Service Navigation:** Reduce reliance on asking passersby from our **75.0% baseline** to under **25%** users who can navigate on their own.
- **Directory Accuracy:** Fewer than **10%** of searches result in reported wrong or outdated room directions.
