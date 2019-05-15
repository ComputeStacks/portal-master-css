# Stylesheets for ComputeStacks Cloud Portal

## Image Formats
Login Logo: 200 x 100 (W x H)
In-App Nav Bar: Max height of 32px. Width can be any size, but should not exceed 260px.
In-App Admin Nav Bar: Same as above.

## How to customize
If we have already setup a unique git repo for you, clone from that using `git clone <url>`. Otherwise, clone our master repo and create your own repository with:: 

  1. `git clone -o master https://github.com/ComputeStacks/portal-master-css.git computestacks-css`
  2. `git remote add origin <your new git repo> && git push --set-upstream origin master`

Make your changes in `theme/vars.scss`

Once you've made the changes, and `git push` the changes, open a ticket with ComputeStacks and we will update your CloudPortal.

### Compile
If you would like to compile the changes yourself, please follow these instructions.

First, make sure you have the following installed:

* sass - `gem install sass`
* sass-globbing - https://github.com/chriseppstein/sass-globbing - `sass-globbing`

Then run the following command:

    sass -r sass-globbing -t compressed application.css.scss src/application-1.css


### Example:
    sass -r sass-globbing -t compressed application.css.scss src/application-0.css
