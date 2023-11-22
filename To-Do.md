# To Do List:

- Build UI for logging workouts / sets / reps 

- Render a list? How to structure list though? My pen and paper workout logs are just:
 ( Date - Activity )
 11-1-23 Leg day

 Followed by sets and reps with name of each 
 exercise: 

 Squats: 

Set 1: 245 x 10

so first set is 245 pounds with 
10 repetitions

How would I structure this to mimic my pen and paper logs? 

Add workout button first which will create a modal popup 
maybe asking for date, leg / ab day, back / biceps, chest / tri / shoulders, cardio day

Then that will create a list component maybe that will have 
an add exercise button, which has another modal asking 
for name of exercise like squat or calf raises, then the set and rep..

Should the main UI just be a calendar? Or maybe just render a calendar which will have references to those workout days 
and on click brings up info? 

Maybe start with just rendering a list?

3. Setting Up MongoDB
This step is the same as in the previous explanation. Choose between local MongoDB or MongoDB Atlas, install Mongoose, and set up a connection utility.

4. Basic CRUD Operations
No changes here. Implement CRUD operations for your workout logs by creating a schema, setting up API routes in Next.js, and handling data operations.

Add Workout Button: When clicked, it opens a modal to add a new workout session.
The workout list can be structured with components such as:

Box or Flex: For layout structuring.
List: To display each workout session.
ListItem: For each workout entry.
2. Adding a Workout
When the user clicks the "Add Workout" button, display a modal that allows them to enter details like:

Date
Workout Type (e.g., Leg Day, Cardio Day)
You can use:

Modal: For the popup.
Input: For entering details.
Select: For workout type selection.
3. Displaying Workout Details
Each workout session can expand to show details like exercises, sets, and reps. For this, you can use:

Accordion: To toggle visibility of each workout's details.
Table: To neatly display sets and reps for each exercise.
4. Adding Exercises to a Workout
Within each workout's details:

Add Exercise Button: Opens a modal to add exercises to that workout session.
Form: In the modal, to enter exercise name, sets, and reps.
5. Calendar View (Optional)
Consider adding a calendar view if you want a more visual representation of workout days. This could be a separate page or a view toggle on the main page. You would use a:

Calendar Component: Display workout sessions on a calendar.
6. Setting Up MongoDB
Set up your MongoDB schema to reflect the structure of your workouts. This might include models for:

Workout Session: With fields for date, type, and a reference to exercises.
Exercise: With fields for name, sets, reps.
7. CRUD Operations
Implement the CRUD operations for:

Creating a new workout session.
Adding exercises to a session.
Updating and deleting exercises or sessions.
8. Frontend and Backend Integration
Connect your frontend components with your Next.js API routes.
Ensure your API interacts correctly with the MongoDB database.
9. Styling and Responsiveness
Use Shadcn UI's styling capabilities to make your application visually appealing and responsive.

Start with Rendering a List
Since you're more accustomed to a list format, start with rendering a simple list of workouts. Once this basic functionality is in place, expand to include more features like the calendar view or detailed exercise logging.

