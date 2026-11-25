# Product Requirements Document (PRD)

**Product Name**: CAMPUS NAVIGATION SYSTEM 
**Course**: BU-COS 209   
**Team**: Group 6 (`BU-COS-209-GROUP-6`)  

1. Product Overview
This is a Navigation system that helps, incoming students, regular students, staff, visitors and even parents to be able to find their way around the campus easily no matter where it is.

## 2. Problem Statement & User Research
**The Problem**
From the research conducted, it was found out that some of the interviewed campus users has had some bad experience, either lateness to class, failure to locate a particular building, and so on.

### Primary Research Findings (Survey = 8 users)
To validate this problem, our team surveyed 8 campus community members across different groups (100-level fresher, returning students, postgraduate student, lecturer/staff, and a visitor/parent).

**Research Metric** 
| **Lateness due to navigation** | **62.5%** (5 out of 8) arrived late to a class, exam, or appointment | Poor wayfinding directly harms punctuality |
| **Current coping habit** | **75.0%** (6 out of 8) ask passersby, security, or porters first | High reliance on informal, error-prone human help |
| **Hardest locations to find** | **62.5%** (5 out of 8) struggle with indoor lecture halls/classrooms | Pinpointing a building exterior is not enough |
| **Most requested help** | **62.5%** (5 out of 8) want step-by-step landmark directions | Users prefer visual landmarks over raw coordinates |

### Real User Experiences (Survey Quotes)
> "When I got to a location and I was told that it was the wrong place. Only to be directed to another place and it still was the wrong location. I was just going in circles, and eventually the first place was actually where I was supposed to go."  
> — *Postgraduate Student (3+ years on campus)*

> "Walking to a different place and later finding out it was closer than where we went."  
> — *Returning Student (200-Level & above)*

### Why Existing Solutions Fall Short
- **Standard Map Apps (e.g., Google Maps):** As much as google maps sounds like a solution, it falls short because not every person in the campus community has an access to active mobile internet and also the school wifi might not also be effective everywhere.
  Secondly, the user, might not know the name of where he/she is going as to search on the map.
- **Asking Passersby / Security:** A passerby might also not know the name of the place and also it affects your timing to your specific appointment when you keep stopping from time to time to inquire about direction.

## 3. Proposed Solution
A system where the campus community can be able to find their way easily using landmark-based walking directions, a specific search for each building on campus, and also a campus directory that is easy for even a visitor to read.

## 4. Target Users
- **New & Returning Students:** Especially 100-level freshers navigating their way through lecture and administrative halls.
- **Campus Visitors & Parents:** Those who do not know the buildings by their nicknames or the shortcuts.
- **Campus Administrators / Student Reps:** Those who maintain building records, room allocations, and gate schedule.


## 5. MVP Scope & Features

### In-Scope (Version 1 MVP)
1. **Keyword & Nickname Search:** [Describe in 1 sentence.]
2. **Building-to-Room Directory:** [Describe in 1 sentence.]
3. **Landmark-Based Walking Directions:** [Describe in 1 sentence.]
4. **Operating Hours & Gate Status:** [Describe in 1 sentence.]
5. **Admin Venue & Closure Management:** [Describe in 1 sentence.]

### Out-of-Scope (Future Versions)
- [List 2–3 features you are saving for later, e.g., live turn-by-turn GPS voice navigation, indoor AR arrows, or campus shuttle tracking.]

---

## 6. Detailed Requirements, User Stories & Acceptance Criteria

### Feature 1: Alias & Nickname Search
- **User Story:** As a [user type], I want to [action] so that [benefit].
- **Acceptance Criteria:**
  - [Condition 1 that must be true for this feature to work]
  - [Condition 2, e.g., handling partial matches or slow mobile internet]

### Feature 2: Hierarchical Indoor Location Data
- **User Story:** As a [user type], I want to [action] so that [benefit].
- **Acceptance Criteria:**
  - [Condition 1, e.g., displays Building -> Floor -> Wing -> Room description]
  - [Condition 2, e.g., includes entrance or landmark photos]

### Feature 3: Landmark & Footpath Walking Directions
- **User Story:** As a [user type], I want to [action] so that [benefit].
- **Acceptance Criteria:**
  - [Condition 1, e.g., routes include pedestrian shortcuts]
  - [Condition 2, e.g., uses visible campus landmarks instead of street names alone]

### Feature 4: Operating Hours & Access Status
- **User Story:** As a [user type], I want to [action] so that [benefit].
- **Acceptance Criteria:**
  - [Condition 1, e.g., shows whether a building or shortcut gate is currently Open or Closed]

### Edge Cases Handled
- **Poor Internet Connectivity:** [Explain how the system still delivers basic text directions on slow data.]
- **Duplicate Room Numbers:** [Explain how the system separates "Room 101" in two different buildings.]
- **Closed Gates After Hours:** [Explain what happens when a shortcut closes in the evening.]

---

## 7. Success Metrics
- **Active Searches:** [Target number of weekly student/visitor lookups]
- **Reduction in Lateness:** Reduce venue-related lateness from our **62.5% survey baseline** to under **[X]%**.
- **Self-Service Navigation:** Reduce reliance on asking passersby from our **75.0% baseline** to under **[X]%**.
- **Directory Accuracy:** Fewer than **[X]%** of searches result in reported wrong or outdated room directions.
