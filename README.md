# CAASPP ELA Practice Computer Adaptive Task Portal

This portal acts as a repository of CAASPP-style ELA Computer Adaptive Tasks (CAT). CAT passages are provided for grades 3, 4, 5, and 6.

## Features

### Designed around local storage

Students can access the activity and work on it over several sessions. Their work is saved in browser storage, so as long as they are using the same device, they will have access to their own work.

The expected workflow for a student can be something like the following:

* Share a link to the assignment in Google Classroom along with a Google Doc (created with "Each student gets a copy").
* The student works on their CAT activity. They may save their responses to each question as they proceed (which locks their answer) or work through all the questions before clicking "Review & Turn In".
* At the "Review & Turn In" stage, any multiple choice questions are automatically graded. The student is given a modal from which they can copy their formatted responses and paste it into the Google Doc for submission.
* Note that open response questions aren't automatically graded. Instead, they are added to the top of the information to be copied so it's easy for the teacher to see what work needs to be manually graded.

### Easy to customize

Each assignment comprises a pair of files: a `.json` file and a `.md` file. Both files should have the same name minus the file extension.

* The `.json` file contains the questions for the CAT assessment. This is parsed and displayed on the right of the screen with each question as a "tab".
* The `.md` file contains the text that is displayed on the left of the screen.

The following gist should help converting Google Forms into a plug-and-play json file (or it should at least help get you close to your needed output): https://gist.github.com/mrdwab/e06a58a2b3124095d7eacb31959ee8aa

Remember to update `catalog.json` with the name of any new pair of files added. Following the naming convention means the tasks will automatically be added to the dropdown menus created in `index.html`.

### Convenient printing

If you prefer working with paper copies, the repository can also be used to print out the articles in a nicely formatted packet. The print feature currently creates a packet with:

* The reading passage formatted in two columns for easier reading.
* The questions with radio buttons, checkboxes, and a space for writing short answers.

For the most part, you should be able to just print without changing any settings; from time to time, you may need to adjust the page scale if there are any orphaned lines that you'd like to adjust for.