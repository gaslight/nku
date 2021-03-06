# Assignment scores

due: 3/21/2014

**Creating assignments**

``` As an administrator I want to give assignment grades to students so that
students can know their scores for each assignment ```

1. When signed in as an admin user, an administrator sees a link to create a new
   assignment

2. Clicking the new assignment link takes them to the assignments/new page

3. On the assignments/new page, the user sees an assignment form with the fields:
  * "Student" - select box to choose a student from all the students in the
    database
  * "Name" - the name of the assignment (example: "Assignment 3 - Bueller needs
    a password")
  * "Score" - the number of points the student scored on the assignment
  * "Total" - the total possible points for the assignment

4. Submitting the form creates an assignment for the selected student and
redirects the user back to the students index page

5. Non-admin users who attempt to visit the assignments/new page will be
redirected to the homepage with a flash message saying: "Unauthorized"

**Notes:**

You can either add an attribute to your current Student/User model to
indicate that they are an administrator or you can create a new model.

``` As a student I want to see my scores for each assignment so that I can know
how I'm doing in the class ```

1. When signed in as a student, the student sees the link "My Assignments"

2. Clicking the link takes the student to the assignments/index

3. On the students index page, the student sees a table with the following
columns
  * "Name" - the name of the assignment
  * "Score" - the number of points the student scored on the assignment
  * "Total" - the total possible points for the assignment
  * "Percentage" - the calculated percentage grade on the assignment (example:
    13/15 = 87%)

``` As a student I don't want other students to see my grades so that they don't
find out how well I'm doing and resent me ```

1. If a student tries to view another's grades by changing the URL, they are
   somehow prevented from seeing them.

``` As a student I want to see my current grade for the class so I always know
how I'm doing ```

1. When a student views their list of assignments, they see their current
   average grade for the assignment labeled: "Current Grade".

``` As an administrator I want to see students grades so that I know how they
are doing in the class ```

1. When signed in as an administrator I click on "All Assignments" and I see a list
   of all the assignments in the system.

2. When I select a student from a select control and hit filter, I only see
   grades for the student that I selected.
