---
layout: posts
title: Django Project
---

## Football School

Welcome to the Football School blog! In this Django project, we're building a platform to share insights, updates, and information about our football school. Let's take a look at the key functionalities of our Django views in the `views.py` file.

1. **`gallery_page`**:
   - Role: Display a gallery page.
   - Function: Utilizing Django's `render` function, the HTML page related to the gallery is presented to the user.

2. **`teams`**:
   - Role: Display a page about teams.
   - Function: Using Django's `render` function, the HTML page related to teams is presented to the user.

3. **`about_us`**:
   - Role: Display a page about us.
   - Function: Using Django's `render` function, the HTML page related to about us is presented to the user.

4. **`landing_page`**:
   - Role: Display the main landing page with various information.
   - Function: Initially, an instance of `LandingPage` is obtained from the models. If the request method is GET, a simple search is performed, and the results are passed to the template.

5. **`enter_personal_info`**:
   - Role: Handle the submission of personal information.
   - Function: If the request method is POST, the data entered by the user is received as a `PersonalInformationForm`, and if valid, it is saved to the database. Otherwise, the form is displayed to the user for correct input.

6. **`Under 8`**, **`Under 9`**, **`Under 10`**:
   - Role: Display information about practice, coaches, and players, respectively.
   - Function: Data related to practice, coach, and players are retrieved from the corresponding models and sent to the respective HTML pages.


Feel free to explore our Football School blog and stay tuned for the latest updates and insights!<br>
<a href="http://fkhalili84.pythonanywhere.com">football school</a>
