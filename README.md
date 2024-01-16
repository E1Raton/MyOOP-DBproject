# The Horseland stud
An app which allows you to perform the following actions: 
  * log in to your account
  * create an account (in case you don't have) - sign up
  * see reviews of the horses belonging to the stud
  * program a horse riding course (only for students)
  * cancel a future horse riding course already planned (only for students)
  * submit a review for a horse (only for students)
  * see all the courses (only for instructors)

## User manual
### 1. Log in
This is the first window that appears when running the application. It provides a *welcome* message, two annotated fields for typing the credentials (e-mail address and password), the *Log In* button, the *Sign Up* button and the *See Reviews* button. Trying to log in with wrong credentials (i.e. that can't be found in the database will result in an error message, saying *Invalid e-mail or password*.
### 2. Sign up 
Upon pressing the *Sign Up* button, a *sign up* form opens, having four fields: *First Name*, *Last Name*, *e-mail*, *password* and 2 choice boxes: *Student* and *Instructor* (you can select only one). If you press *Sign In* before completing all these fields or before making a choice between student and instructor, a corresponding error message occurs. This also goes for typing an already registered e-mail address. In case of a successful sign in, the user goes automatically back to the *log in window*. At any time, the user can abandon the *sign up process* by clicking on *Go Back*.
### 3. Reviews Display
This window is reachable from the *log in* window (by clicking on *See Reviews* button). All reviews submitted until now are displayed here in a *TableView*. Additionally, the user has the possibility of sorting the reviews after the name of the horse, a feature which enables you to have a more organised view. You can return to the *log in window* by pressing on *Go Back*.
### 4. Logged in user
Depending on your account (student/instructor) the app redirects you to a certain *scene* from where you can perform your specific actions.
 * **Student**<br></br>
The opened window provides you with three options (buttons): *Program Course*, *See my courses*, *Review*:
 * *Program Course* opens a form where you have to set the details for the horse riding course: select a category, an instructor, a horse, a date, and a starting hour. Be aware of some constraints: you cannot leave an empty field, you cannot choose a past date, you cannot pick a horse which is already picked at in that date, at that hour. Violating any of these will result in some corresponding error messages.
 * *See my courses* redirects you to a *scene* where your courses can be displayed. Just press on *Activated courses* to see the past courses, and on *Future courses* to see the future courses. You can cancel a future course by selecting the course and pressing the *Cancel* button from below. A pop-up window will appear, asking if you are sure you want to perform this action. You can either click *OK* - so the action will be done, or *Cancel* - to prevent the deleting of the course. This option is available only for the future courses, don't try to cancel courses from a past date - the app won't permit it.
 * Press *Review* if you want to leave us a review for one of the horses. Please take into account that you can review a horse only once. In case you try to review the same horse a second time, an error message will occur. Don't try to submit an empty review, or a review without a grade assigned. Error messages will appear in these cases too, and you won't be able to submit the review.
<br></br>
<br></br>
 * **Instructor**<br></br>
A view of all the courses will appear. You can filter by checking *Show only future courses*. You can sort the courses by: *Instructor*, *Student*, *Horse*, *Date*, and *Hour*. Besides, you can search a course by the name of the instructor: just press some key characters followed by *Enter*. This is useful if you wish to see only your courses, or only the courses of one of your colleagues.

Both student/instructor users are provided with a an option (a button) for returning to the *log in window*.

## Future developments
* creating an *admin* account for **complete** database management
* adding an option (for both instructor and student) which enables them to register their horses
* allowing students to register in competitions
* displaying charts which shows the score of each horse, based on the grades given by users
* adding images for each horse (even for users)
* application deployment

## Resources
* *IntelliJ IDEA* + *JavaFX*: Java code for database management, development of the involved classes - mapped entities (from database), database controllers, scene controllers, .fxml files, utilities classes.
* *DBeaver* + *PostgreSQL*: database design
* *JDBC*: connection to database (between the Java code and the database)
