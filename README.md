

### Set-up steps

Following [this guide](https://nicolas.perriault.net/code/2012/dead-easy-yet-powerful-static-website-generator-with-flask/).

```
mkdir sample_project && cd $_
virtualenv venv
source venv/bin/activate
pip install Flask Frozen-Flask Flask-FlatPages
touch sitebuilder.py
# add content
python sitebuilder.py
# visit localhost:8000
mkdir pages
touch pages/hello-world.md
# add page content
mkdir templates
touch templates/base.html
# add content
touch templates/page.html
# add content
touch templates/index.html
# add content
touch templates/tag.html
# add content
touch templates/_list.html
# add content
```

####Virtual Env and Requirements Text
Don't check the virtual environments directory into git.  Instead use the requirements text file to manage required packages.
```
pip freeze > requirements.txt
pip install -r requirements.txt
```

####Gitignore
Example .gitignore file for use with virtual env's on OS X
```
# Virtualenv
# http://iamzed.com/2009/05/07/a-primer-on-virtualenv/[Bb]in
.Python
[Ii]nclude
[Ll]ib
[Ll]ib64
[Ll]ocal
[Ss]cripts
pyvenv.cfg
.venv
pip-selfcheck.json

# Mac OS X custom attribute files
.DS_Store
```