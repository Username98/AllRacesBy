# Belarus Running Events Aggregator

## Project Description

This ASP.NET Core application aims to be a comprehensive platform for aggregating, filtering, and showcasing various running events across Belarus. It will cover a wide range of event types, including:
  * Road Races: Marathons, half-marathons, 10k, 5k, etc.
  * Trail Runs: Off-road races in natural environments.
  * Obstacle Course Racing (OCR): Events combining running with various physical obstacles.
  * Training Runs: Regular, often free, community-organized training sessions.
  * Duathlon: Running and cycling events.
  * Triathlon: Swimming, cycling, and running events.
  * Multimarathon: Events with multiple stages or ultra-long distances.
  * Adventure Races: Team-based, multi-day events involving navigation, trekking, cycling, paddling, and other outdoor disciplines.
  * Road Cycling Races: Competitions on paved roads.
  * Mountain Biking (MTB) Races: Competitions on off-road terrain.
  * Swimming Events: Open water swims.
  * Orienteering: Navigation-based races using a map and compass.

The primary goal is to provide a centralized hub for runners in Belarus to discover upcoming events, manage their preferences, and potentially track their participation.

## Core Features

The service will be designed to:
1.  **Procure Event Information:** Gather details about running events from various sources (e.g., official race websites, registration platforms, running club communities).
2.  **Extract Key Details:** Distill essential information for each event, such as:
    *   Event Name
    *   Date and Time
    *   Location (City, specific venue)
    *   Distances offered
    *   Event Type (Road, Trail, OCR, Training)
    *   Registration Link / Official Website
    *   Brief Description
    *   Participation Cost
    *   Organizer
3.  **Store Securely:** Safely store all collected event data within the service's infrastructure.
4.  **User-Facing Platform:** Provide users with visibility into events, allowing them to filter and sort based on configurable criteria (e.g., event type, distance, location, date, price).
5.  **Personalized Preferences (for authorized users):** Allow registered users to customize filtering metrics to align with their preferences (e.g., "show only trail runs in Minsk").
6.  **Administrative Interface:** Equip administrators with tools to manage ongoing operations, such as adding/editing/deleting event information, managing data sources, and potentially user management.

## Additional Features (Optional)

1.  **User Accounts & Favorites:**
    *   Users will be able to register and log in.
    *   Authenticated users can mark events as "favorites" to easily track races they are interested in.
    *   A dedicated "My Favorites" section will be available in the user's profile.
2.  **Personal Race Results & Statistics Tracking:**
      * **User-Submitted Results:** Authenticated users will have the ability to manually input their results for events they've participated in (e.g., finish time, overall place, age group place, specific discipline times for multisport events).
      * **Personal Statistics Dashboard:** 
 The platform will automatically generate and display various statistics based on user-submitted results for a selected period (e.g., year, month, custom range). This could include:
        * Total number of events completed.
        * Average finish place across all events or specific types.
        * Best times achieved on specific distances (e.g., fastest 5k run, 10k run, half-marathon, full marathon).
        * Total distance covered in running, cycling, or swimming events for a given period.
        * Visualizations (charts/graphs) of progress over time.
3. **Automated Race Difficulty Assessment:**
    *   The system will automatically calculate and assign a difficulty level (e.g., "Easy", "Moderate", "Challenging", "Extreme") to each event.
        This assessment will be based on a multitude of parameters, which may include:
        *   **Distance:** Longer distances generally imply higher difficulty.
        *   **Elevation Gain/Loss:** Significant elevation changes (especially for trail runs and MTB) increase difficulty.
        *   **Terrain Type:** Road vs. trail vs. OCR obstacles.
        *   **Event Duration/Format:** (Fixed Duration:, Backyard Ultra, Multi-day events)
        *   **Time of Day:** (Night Race)
        *   **Weather Conditions (historical/typical for date):** Extreme heat, cold, or precipitation can increase difficulty.
        *   **Number of Disciplines:** Multisport events are inherently more complex.
        *   **Historical Participation/Finish Rates:** Lower finish rates or fewer participants might suggest higher difficulty.
        *   **User Ratings/Feedback (future):** Potentially incorporate user-generated difficulty ratings.
    •   This feature will help users quickly gauge if an event matches their current fitness level and experience.

## Technologies Used (Initial Plan)

*   **Backend:** ASP.NET Core
*   **Database:** MSSQL Server 
*   **ORM:** Entity Framework Core (Code First approach)
*   **Frontend:** (To be determined, potentially Razor Pages or a JavaScript framework like React/Angular)
