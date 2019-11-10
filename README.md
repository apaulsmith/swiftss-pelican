# SWIFTSS Website
The homepage website for the SWIFTSS charity, hosted at https://www.switftss.org

## Implementation
The SWIFTSS website is a statically generated using [Pelican](https://getpelican.com). [Bootstrap](https://getbootstrap.com) is used as the front-end component library. The code is maintained in GitHub and licensed under GPL v3. VirtualEnv is used to maintain Python dependencies.

## Getting and building the site locally

Clone the source code from GitHub
~~~~
$ git clone https://github.com/apaulsmith/swiftss-pelican.git
$ cd swiftss-pelican
~~~~

Install virtualenv, create a new environment, and install the required dependencies
~~~
# From inside the 'swiftss-pelican' directory created by git clone
$ pip install virtualenv
$ virtualenv venv

$ venv\Scripts\activate [Windows]
$ source venv/bin/activate [Linux/Mac]

$ pip install -r requirements.txt
~~~

Preview the site
~~~
$ pelican --listen
~~~

And go to http://localhost:8000/ in your browser.

Or build the site
~~~
$ pelican content
~~~

This generates the site inside the `output/` directory.


##Editing the site content
The site content is a set of [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#emphasis) files inside the `content/` directory.


##Deploying updates to the site
The application is deployed to a S3 bucket.

*_Instructions to follow..._*
