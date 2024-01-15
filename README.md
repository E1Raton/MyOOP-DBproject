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
 * **Student**


The opened window provides you with four options (buttons): *Program Course*, *See my courses*, *Review*, and *Log Out*.
 * **Instructor**
