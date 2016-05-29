# Mucking with StaticAid
Can I setup my own version of Helrond's StaticAid for PSU Special Collections?

What I want to do:
* Use a script to grab ASpace records via the API
* Deposit ASpace records in GitHub for version control
* Create static HTML site for finding aids
* Automate all this

## Journaling my steps:
* python --help -- Hey, I already have the correct version of Python. Fuck yes.
* pip install requests -- Looky here, I already have pip installed, so that makes shit easier. And what do you know, "Requirement almost satisfied."
* pip install requests-toolbelt -- Success
* pip install psutil -- Success
* gem install jekyll -- easy, mr hyde
* Node package manager -- ok, things get a little less straightforward for my inner hippie luddite. Made my way to https://nodejs.org/en/ and 
installed v4.4.5 for MacOSX. 
* node -v' -- yes, it's there. Score.
* sudo npm install npm -g -- Yup.
* npm install -g grunt-cli -- ERROR. Didn't have permissions to /usr/bin/local or some such. So do I need to add 'sudo'?
* sudo npm install -g grunt-cli -- Hey, I think that worked.
