# Project Name: CoLocate
## Project Overview
CoLocate is a test project aimed at increasing intentionality and information in regards to colocating in the office through intelligent calendar event and space management. It comprises a set of tools and scripts designed to generate, analyze, and recommend when time in person is a worthwhile idea. The project aims to help individuals and teams make the most of their time by optimizing office interactions and facilitating meaningful collaboration.

## Features
### 1. Event Generation Script
**Random Event Generation:** Create a variety of events with different parameters (collaborative, expected number of attendees, expected duration, etc.) within arbitrary time blocks for an arbitrary number of people within an arbitrary number of teams. These events will be used as test data for a MVP. Alternatively, an organization's calendars could be imported using RESTful API calls to Google Calendar or Microsoft Outlook.

    TO DO: 
        Build API access to Calendars.
        Build event generator (ics on python, default events can be defined using a CSV, functionality to adjust these defaults in individual cases)
        Can they define new events? Would be as simple as picking parameters from a list in their own configuration

**Collaborative vs. Non-Collaborative:** Distinguish between collaborative and non-collaborative events, with collaborative events having other attendees and non-collaborative events typically having no other attendees. Events can also be tagged as being open to drop-ins and people interested in learning more.

### 2. Office Generation Script
**Random Office Generation:** Create offices of varying sizes and containing varying sets of rooms that are able to support an arbitrary amount of people. 

    TO DO:
        Build room definitions, similar to events
        Size is selected, small = ~5 rooms, medium = ~10 rooms, large = ~15 rooms. Discrete set layouts prepared ahead of time, 3 of each and is selected randomly. 
        
### 3. ML-Based Recommendation Script
**Intelligent Event Comparison:** Use machine learning to compare and analyze events to provide recommendations on when to colocate and what office space to use. Additionally provide recommendations on when it would make sense to shift schedules in order to stack colocated events on a single day, so it is used more effectively.

    TO DO:
        Build AI (so easy right?). MVP can just perform API calls to GPT3.5 to act in this manner after a bit of train, more robust effort would be to build something ourselves.
        
**Recommendations:**
Suggest days suitable for colocating with team members based on meetings together.
Identify opportunities to merge social events with other teams.
If many colocated meetings are sporadic across the week, suggest changing them to be on a single day.

### 4. User-Friendly Front End
Interactive Interface: Develop a front end that allows users to utilize the event generation and recommendation scripts. Calendar and list of people to see the events generated for them. Pop in suggestions to change things. MVP, no need for this to be interactable.
Parameter Adjustment: Enable users to adjust parameters for event generation and analysis, including rate at which meetings occur interteam and percentage of workday occupied by meetings.

## Development Steps
To bring the CoLocate project to life, the following steps will be taken:

### Event Generation Script:

Create a script that generates random events within specified constraints.
Implement event type selection and collaborative/non-collaborative event generation.
Ensure that team dynamics are considered when scheduling collaborative events.

### ML-Based Recommendation Script:

Develop a machine learning model to analyze and compare generated events.
Train the model to make recommendations, including suitable days for colocating and opportunities to join other teams' events.

### User-Friendly Front End:

Design and build an interactive front end for users to access the project's functionalities.
Enable users to adjust event generation parameters and receive recommendations.

### Testing and Validation:

Thoroughly test the scripts and front end to ensure accuracy and usability.
Gather user feedback and make necessary improvements.

### Documentation and Hosting:

Create comprehensive project documentation that explains the project's purpose, features, and usage.
Choose a hosting platform (e.g., GitHub or a personal website) to make the project accessible to others.

## Conclusion
CoLocate is an exciting project that aims to transform office collaboration by optimizing event scheduling and offering intelligent recommendations. We look forward to bringing this innovative tool to life and helping individuals and teams make the most of their time in the workplace.

