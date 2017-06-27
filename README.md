# psadmin.io Fluid Stylesheets

These styles are Fluid versions of the psadmin.io 8.54 and 8.55 Classic stylesheets.

## Installation

These styles are delivered as a Data Migration project. Use the Data Migration Workbench to load the updated styles.

1. Download the latest [`IO_STYLES_FLUID.zip`]()
1. Unzip the `IO_STYLES_FLUID.zip` to your Data Migration file location.
1. Navigate to PeopleTools > Lifecycle Management > Migrate Data > Data Migration Workbench
1. Select "Load Project From File"
1. Select the file location and the `IO_STYLES_FUILD` project. 
1. Select "Submit Project for Copy"

After the Migration Project is loaded, change the theme for your application.

1. Navigate to PeopleTools > Portal > Branding > Branding System Options
1. Select the `IO_THEME_xxx` you want.
1. Click OK. 
1. Log out and log back in to see the changes.

## Change the Logo

To change the logo, you can upload a new image file to use.


## Create a new Theme

1. [Pick a main color here](https://www.w3schools.com/colors/colors_picker.asp)
1. Select the supporting colors for the theme:
    * Main 
    * Light (5-10% lighter)
    * Dark  (5-10% darker)
    * Border (20% darker)
    * Hover (5% darker than Dark)
    * Active (5-10% darker than Hover)
1. Clone `IO_BRAND_FLUID_TEMPLATE_BLUE.css`
1. Update the colors in `IO_BRAND_FLUID_TEMPLATExxx.css`
1. Upload the new stylesheet via Branding Objects > Stylesheets as `IO_BRAND_FLUID_TEMPLATE_xxx`
1. Clone the `IO_*_BLUE.svg` files to your new color
1. Edit the `.svg` files to use the main color.
1. Upload the new images via Branding Objects > Images
1. Clone the Macro Set `IO_THEME_BLUE` to `IO_THEME_xxx`
1. Change the colors in the new Macro Set
1. Change the image names to the new colors
1. Assemble a new theme by saving `IO_THEME_BLUE` as `IO_THEME_xxx`
1. Change the Homepage Header, Macro Set, and Fluid Global Override Stylesheet
1. Change the Default Branding to use the new theme.
1. If needed, use the Assign Theme page to change role assignments to use the new theme.


