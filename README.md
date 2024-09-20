Lab Workflows Automation
========================

[![Deploy Jekyll site to GitHub Pages](https://github.com/anjal-amin/lwf/actions/workflows/jekyll.yml/badge.svg)](https://github.com/anjal-amin/lwf/actions/workflows/jekyll.yml)

Website reporting latest solutions for labs automating their procedures.

Pulling the Repository
----------------------

To get started with the repository, clone it using:

````bash
git clone https://github.com/anjal-amin/lwf.git
cd lwf
````

Build the Site Locally
----------------------

Before building the site, make sure you have Ruby and Bundler installed. 

* On Ubuntu
** do NOT install the snap version of ruby.
** after installing bundler: `bundle config path ~/.local/ruby-gem` # or pick your own random ruby-gem location

If not, you can install them using the following commands:

````bash
# Install Bundler
gem install bundler
````

Once Bundler is installed, use it to install the necessary gems:

````bash
bundle install
````

To build the site locally and view it, use:

````bash
# Build the site
bundle exec jekyll build

# Serve the site locally
bundle exec jekyll serve
````

Your site will be available at <http://localhost:4000>.

Deploy the Site
---------------

### GitHub Pages Deployment

To deploy the site to GitHub Pages, you can use the GitHub Actions workflow defined in `.github/workflows/jekyll.yml`. This workflow will automatically build and deploy the site whenever changes are pushed to the `main` branch.

### Manual Deployment

To manually deploy the site to GitHub Pages, follow these steps:

1.  Make sure you have committed your changes.

2.  Push your changes to the `main` branch:

````git add .
git commit -m "Describe your changes"
git push origin main`
````
GitHub Actions will handle the build and deployment process for you.

License
-------

This project is licensed under the MIT License - see the LICENSE file for details.

Contributing
------------

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes. We welcome contributions and appreciate your interest in improving this project!

For more detailed documentation, please visit the [Jekyll documentation](https://jekyllrb.com/docs/).
