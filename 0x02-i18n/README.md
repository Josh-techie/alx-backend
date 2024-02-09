<p align="center">
<img src ="https://i.redd.it/8phjnjk6rjd41.png">
</p>

---

<h2> 0x02. i18n </h2>

- This project focuses on internationalization and localization (i18n) in a Flask web application. The goal is to create a multi-language web application that can display content in different languages based on user preferences, URL parameters, and other factors.

---

<h2> Resources </h2>

- [Flask-Babel](https://pythonhosted.org/Flask-Babel/)
- [Flask i18n tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xi-i18n-and-l10n)
- [pytz](https://pythonhosted.org/pytz/)

---

<h2> Tasks </h2>

0. **Basic Flask app:**

   - **Description:** Set up a basic Flask app in `0-app.py`. Create a single / route and an `index.html` template that outputs "Welcome to Holberton" as the page title `(<title>)` and "Hello world" as the header.
   - **File:** [0-app.py](./0-app.py), [templates/0-index.html](./templates/0-index.html)

1. **Basic Babel setup:**

   - **Description:** Install the Babel Flask extension using `$ pip3 install flask_babel==2.0.0`. Instantiate the Babel object in your app and store it in a module-level variable named `babel`. Create a Config class with a `LANGUAGES` class attribute equal to ["en", "fr"]. Use Config to set Babel’s default locale ("en") and timezone ("UTC").
   - **File:** [1-app.py](./1-app.py), [templates/1-index.html](./templates/1-index.html)

2. **Get locale from request:**

   - **Description:** Create a `get_locale` function with the `babel.localeselector` decorator. Use `request.accept_languages` to determine the best match with supported languages.
   - **File:** [2-app.py](./2-app.py), [templates/2-index.html](./templates/2-index.html)

3. **Parametrize templates:**

   - **Description:** Use the `_` or `gettext` function to parametrize your templates. Use message IDs `home_title` and `home_header`. Create a `babel.cfg` file and initialize translations with pybabel. Edit translation files for English and French. Compile dictionaries and ensure correct messages show up on the home page.
   - **Files:** [3-app.py](./3-app.py), [templates/3-index.html](./templates/3-index.html)

4. **Force locale with URL parameter:**

   - **Description:** Implement a way to force a particular locale by passing the `locale=fr` parameter to your app’s URLs. In your `get_locale` function, detect if the incoming request contains the `locale` argument and its value is a supported locale.
   - **Files:** [4-app.py](./4-app.py), [templates/4-index.html](./templates/4-index.html)

5. **Mock logging in:**

   - **Description:** Create a user login system by copying the provided user table in 5-app.py. Define a `get_user` function and use `app.before_request` to set the user as a global on `flask.g.user`. Display a welcome message or default message in the HTML template based on login status.
   - **Files:** [5-app.py](./5-app.py), [templates/5-index.html](./templates/5-index.html)

6. **Use user locale:**

   - **Description:** Change your `get_locale` function to use a user’s preferred locale if it is supported. Test by logging in as different users.
   - **Files:** [6-app.py](./6-app.py), [templates/6-index.html](./templates/6-index.html)

7. **Infer appropriate time zone:**

   - **Description:** Define a `get_timezone` function and use the `babel.timezoneselector` decorator. Find the timezone parameter in URL parameters, get time zone from user settings, and default to UTC. Validate that the provided or user time zone is valid using `pytz.timezone`.
   - **Files:** [7-app.py](./7-app.py), [templates/7-index.html](./templates/7-index.html)

> ### Advanced Task:

8. **Display the current time:**

   - **Description:** Display the current time on the home page based on the inferred time zone in the default format. Use translations for the message ID `current_time_is`. The time should be displayed in the format like "Jan 21, 2020, 5:55:39 AM" or "21 janv. 2020 à 05:56:28" depending on the selected language.
   - **Files:** [app.py](./app.py), [templates/index.html](./templates/index.html)

---

<h2> Author </h2>

- [`@Josh-techie`]() | Software Engineer Student

  > Reach out to me if you need any help or have any questions.

  <a href="mailto:youssef.abouyahia@e-polytechnique.ma">
  	<img alt="Feel free to contact me" src="https://img.shields.io/badge/-Ask_me_anything-blue?style=flat&logo=Gmail&logoColor=white&link=mailto:youssef.abouyahia@e-polytechnique.ma&color=3d85c6" />
  </a>
  <span> | </span>
    <a href="https://www.linkedin.com/in/youssef-abouyahia/">
        <img alt="Linkedin Profile" src="https://img.shields.io/badge/-Linkedin-0072b1?style=flat&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/youssef-abouyahia/" />
    </a>
    <span> | </span>
    <a href="https://twitter.com/JoesephAb">
        <img alt="Twitter Profile" src="https://img.shields.io/badge/-Twitter-0072b1?style=flat&logo=Twitter&logoColor=white&link=https://twitter.com/JoesephAb&color=1DA1F2" />
    </a>
