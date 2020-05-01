# imharshanand.github.io

Website URL: http://anandharsh.herokuapp.com/
Based on https://medium.com/p/991845147ec

Host Static Website to Heroku:
    Add a file called composer.json to the root directory by running touch composer.json
    Add a file called index.php to the root directory by running touch index.php
    Rename the homepage (e.g. index.html) to home.html
    In index.php, add the following line: <?php include_once("home.html"); ?>

    Or use a Profile
        web: node index.js
        
        if PORT is used in the app then
        instead of "var PORT = 5000;" 
        use "var PORT = process.env.PORT || 5000;"

    In composer.json, add the following line: {}
    Run git push heroku master

Commands:
git init
git add .
git commit -m "My site ready for deployment."
heroku apps:create my-static-site-example
git push heroku master

For making changes to already uploded app on Heroku
git add .
git commit -m "Add useful message"
git push heroku master
