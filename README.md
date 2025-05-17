# greenwood-library-website

## Step-by-Step Simulation

### Step 1: Set Up the GitHub Repository

**Create a New Repository on GitHub:**

Go to [ **github.com**](https://) and sign in.

Click the “+” icon in the top-right corner and select “New repository.”

Set the repository name to greenwood-library-website.

Check “Add a README file” to initialize with README.md.

Keep it public or private as preferred.

Click “Create repository.”


 **Clone the Repository Locally:**

Copy the repository URL (e.g., https://github.com/your-username/greenwood-library-website.git).

![alt text](<img/img 2.png>)


Open your terminal and clone the repo:

> mkdir greenwood-library-project

> cd greenwood-library-project

> git clone https://github.com/your-username/greenwood-library-website.git

> cd greenwood-library-website



### Step 2: Create Initial Website Files in the main Branch

We’ll create the basic website files (home.html, about_us.html, events.html, contact_us.html) with random content using VS Code and commit them to the main branch to simulate the existing codebase.

![alt text](<img/img 3.png>)

Open the Project in VS Code:
bash

code .

This opens the greenwood-library-website directory in VS Code.

Create HTML Files with Random Content:

In VS Code, create the following files in the repository root and add simple HTML content:

home.html: copy the code and paste in the file


```html
<!DOCTYPE html>
<html>
<body>
  <h1>Welcome to Greenwood Community Library</h1>
  <p>Explore our collection and join our community!</p>
</body>
</html>
```

about_us.html:

```html
<!DOCTYPE html>
<html>
<body>
  <h1>About Us</h1>
  <p>We are a community-driven library fostering knowledge and connection.</p>
</body>
</html>
```

events.html:


```html
<!DOCTYPE html>
<html>
<body>
  <h1>Upcoming Events</h1>
  <p>Stay tuned for exciting library events!</p>
</body>
</html>
```

contact_us.html:

```html
<!DOCTYPE html>
<html>
<body>
  <h1>Contact Us</h1>
  <p>Email: library@greenwood.org | Phone: (123) 456-7890</p>
</body>
</html>
```

Save all files.

Stage, Commit, and Push to main:
In the terminal, run:

> git add .

> git commit -m "Add initial website files: home, about_us, events, contact_us"

> git push origin main



### Verify on GitHub:
Go to https://github.com/your-username/greenwood-library-website.

Confirm that README.md and the four HTML files (home.html, about_us.html, events.html, contact_us.html) are present in the main branch.

![alt text](<img/img 4.png>)


### Step 3: Morgan’s Work – Adding Book Reviews Section

Morgan will create a book_reviews.html file in a new branch called add-book-reviews, push it to GitHub, and raise a pull request.

Create and Switch to Morgan’s Branch:

> git checkout -b add-book-reviews

![alt text](<img/img 5.png>)

Create **book_reviews.html**:

In VS Code, create a new file book_reviews.html in the repository root with random content:

**book_reviews.html**

```html
<!DOCTYPE html>
<html>
<body>
  <h1>Book Reviews</h1>
  <p>Read what our community thinks about their favorite books!</p>
  <ul>
    <li>"The Great Gatsby" - A timeless classic!</li>
    <li>"1984" - Thought-provoking and intense.</li>
  </ul>
</body>
</html>
```

Save the file


Stage, Commit, and Push to main:
In the terminal, run:

> git add book_reviews.html

> git commit -m "add book reviews section"

> git push origin add-book-reviews

![alt text](<img/img 6.png>)



### Create a Pull Request for Morgan’s Work:

Go to https://github.com/your-username/greenwood-library-website.

You’ll see a prompt suggesting the recently pushed add-book-reviews branch; click “Compare & pull request.” Alternatively, go to the “Pull requests” tab and click “New pull request.”

![alt text](<img/img 7.png>)

Set:
Base branch: main

Compare branch: add-book-reviews

Review the changes (GitHub shows the new book_reviews.html file).

Add a title: “Add Book Reviews Section”

Add a description: “Created book_reviews.html with sample book reviews.”

Click “Create pull request.”

![alt text](<img/img 8.png>)

Merge Morgan’s Pull Request:
In the “Pull requests” tab, open the PR.

Review the changes (confirm book_reviews.html is added correctly).

Click “Merge pull request” and then “Confirm merge.”

![alt text](<img/img 11.png>)

Optionally, click “Delete branch” to remove add-book-reviews from GitHub.

Result: The main branch now includes book_reviews.html

![alt text](<img/img 9.png>)


### Step 4: Jamie’s Work – Updating Events Page

Jamie will update events.html in a new branch called update-events, pull the latest main branch to stay updated, push changes, and raise a pull request.

Create and Switch to Jamie’s Branch:

>git checkout main

>git pull origin main  # Ensure local main is up-to-date

>git checkout -b update-events


![alt text](<img/img 12.png>)


Update events.html:

In VS Code, open events.html and modify it to include new event details, e.g.:

```html
<!DOCTYPE html>
<html>
<body>
  <h1>Upcoming Events</h1>
  <p>Join us for these exciting community events!</p>
  <ul>
    <li>Book Club: Oct 15, 2025 - Discuss "To Kill a Mockingbird"</li>
    <li>Author Talk: Oct 20, 2025 - Meet Jane Doe</li>
  </ul>
</body>
</html>
```


Save the file.



Pull Latest Changes from main:

Since Morgan’s changes (adding book_reviews.html) were merged into main, pull those updates into Jamie’s branch to avoid conflicts:
bash

>git pull origin main

If no conflicts occur, Git will fast-forward or merge automatically (since Jamie only modified events.html and Morgan added a new file, there should be no conflicts).

If a conflict occurs (unlikely here), Git will mark it in events.html. Resolve it by editing the file, then stage and commit:
bash

>git add events.html

>git commit -m "Resolved merge conflict with main"

then Stage, Commit, and Push Changes:

>git add events.html

>git commit -m "Update events page with new community events"

>git push origin update-events

![alt text](<img/img 13.png>)



### Create a Pull Request for Jamie’s Work:

Go to https://github.com/your-username/greenwood-library-website.

Click “Compare & pull request” for the update-events branch or create a new PR manually.

Set:
Base branch: main

Compare branch: update-events

Review the changes (GitHub shows the updated events.html).

Add a title: “Update Events Page with New Events”

Add a description: “Added upcoming community events to events.html.”

Click “Create pull request.”

Merge Jamie’s Pull Request:
Open the PR in the “Pull requests” tab.

![alt text](<img/img 14.png>)


Review the changes (confirm events.html updates).

Click “Merge pull request” and “Confirm merge.”

![alt text](<img/img 15.png>)


Optionally, delete the update-events branch.

Result: The main branch now reflects Jamie’s updated events.html.

![alt text](<img/img 16.png>)


## Conclusion

You’ve successfully completed the Capstone Project by:

Setting up the greenwood-library-website repository on GitHub.

Creating and committing initial website files (home.html, about_us.html, events.html, contact_us.html) to the main branch.

Simulating Morgan’s work by adding book_reviews.html in the add-book-reviews branch, creating a PR, and merging it.

Simulating Jamie’s work by updating events.html in the update-events branch, pulling the latest main to stay updated, creating a PR, and merging it.

Verifying that all changes are correctly integrated in the main branch.

This project demonstrates key Git and GitHub workflows: cloning, branching, committing, pushing, creating pull requests, and merging changes collaboratively. The Greenwood Community Library website now has a new “Book Reviews” section and an updated “Events” page, ready for further enhancements.




