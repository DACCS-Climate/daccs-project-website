# The DACCS Project Website
This site is to give a summary of what the DACCS project is about.  It includes a mission statement, vision statement, a list of the Principle Investigators and a list of the Funders.

# Building the site

Clone the repository at [https://github.com/DACCS-Climate/daccs-project-website](https://github.com/DACCS-Climate/daccs-project-website)

Navigate to the root directory and build the site by running 
```angular2html
python build.py
```

The site files will be automatically built and moved to the `/build` folder.

Navigate to the `/build` folder and start an http server by running
```angular2html
python -m http.server
```
