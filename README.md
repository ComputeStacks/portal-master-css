# Stylesheets for ComputeStacks Cloud Portal

## Image Formats
Login Logo: 200 x 100 (W x H)
In-App Nav Bar: Max height of 32px. Width can be any size, but should not exceed 260px.
In-App Admin Nav Bar: Same as above.

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
