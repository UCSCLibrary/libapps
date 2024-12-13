# LibApps for UCSC Library

This repo holds the custom CSS, javascript, header and footer for UCSC's
LibApps. The main branch is on Bootstrap 3 and currently covers all Libapps,
except for the LibGuides A-Z, which is on the bootstrap5 branch.

## Updating CSS

Styles come from the Library's drupal theme, Spencer. 
Stlyes are maintained and should be copied from the global CSS file at:
/sites/all/themes/spencer/css/global.css

## Updating Javascript

Javsacript also comes from the Spencer theme. It can be found at
/sites/all/themes/spencer/js/spencer.js

Note that most of the code there is legacy and is not copied here.
TODO: separate out global from local scripts.

## Updating the header

To update the header, look at the source code of the main website. Copy
from the `<div class="header">` tag down to the closing div just before the
`<div id="main-content">` tag.

1. Update the URL of the search form. It should look like:
    `<form action="https://library.ucsc.edu/search/results" ... >`

2. Remove the style parameter from all elements. These are applied
dynamically by the javascript.

## Updating the footer

Each Libapp has a separate footer to include the specific login link.
Changes to the global footer should be carefully reproduced on each separate
file.

IMPORTANT: The URL of the newsletter subscription form should also point to 
the drupal site.
