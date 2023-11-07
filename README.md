# The DACCS Project Website
This site is to give a summary of what the DACCS project is about.  It includes a mission statement, vision statement, a list of the Principle Investigators and a list of the Funders.

## Building the site
Clone the repository at [https://github.com/DACCS-Climate/daccs-project-website](https://github.com/DACCS-Climate/daccs-project-website)

Navigate to the root directory, install the requirements, and build the site by running: 
```shell
python3 -m pip install -r requirements.txt
python3 build.py
```

The site files will be automatically built and moved to the `/build` folder.

## To view the site
The files in build directory can be served as a static website. Navigate to the `/build` folder and start an 
http server. For example:

```shell
cd build/
python3 -m http.server 8000
```

This will start a basic http server that can be accessed at http://localhost:8000

(Note that this is recommended for development only)

## Development

This is how the files are arranged in this repo and how to update them in order to develop this website.

- Files in the `static/` directory will be copied to the build directory without modification.
- Files in the `templates/site/` directory will be copied to the build directory after being updated by the template engine
- All other directories in the `templates/` directory will not be copied to the build directory but _will_ be used by the templating engine
  - `templates/layouts/` contains files that should be extended by other template files

The template engine used is [Jinja](https://jinja.palletsprojects.com/en/3.1.x/).
