# Stylesheets for ComputeStacks Cloud Portal

## How to customize
Make your changes in `theme/vars.scss`

Once you've made the changes, and `git push` the changes, open a ticket with ComputeStacks and we will update your CloudPortal.

### Compile
If you would like to compile the changes yourself, please follow these instructions.

First, make sure you have the following installed:

* sass - `gem install sass`
* sass-globbing - https://github.com/chriseppstein/sass-globbing - `sass-globbing`

Then run the following command:

    sass -r sass-globbing -t compressed application.css.scss src/application-${VERSION}.css


###Example:
    sass -r sass-globbing -t compressed application.css.scss src/application-0.css
