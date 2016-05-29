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
* Download the staticAid ZIP file, unpack, move to a projects folder. 
* cd projects/staticAid-master
* npm install
* open local_settings.default -- I'm too lazy (this is why I suck at tech) to look up how to edit a file from the command prompt, so I just opened this file in TextWrangler. 
* There's a section on ASpace that needs to be edited for our own instance. But what is this AdLib section? Do I need to change anything here? I guess I'll ignore it for now and see what happens.
* "Change the values in _config.yml to match your preferences. Make sure to change url and baseurl." UMMMM, where is this file? Let's just keep going...
* grunt update -- because I want to use our own data... Helrond warns this may take awhile. Weirdly, it did not. Is this grabbing our ASpace data or RACs? Let me look at one of the files. Ok, crap, it's a RAC resource record. Let's look at this utilities/getJson.py file. No dice. Nothing here. Hmm. Let's move along with the data that's there...
* grunt serve -- this is taking awhile. Inspecting some of these python scripts while I wait, and I really can't figure out why it's not pulling data from the right ASpace. All signs point to that config file for setting the BaseURL. 
* Site built, and I can access it at localhost:4000, and HEY it's red. 

Okay, I got this far. I have staticAid running. But now need to figure out why it's not grabbing the right ASpace data. 



