# LibApps for UCSC Library

This repo holds the custom CSS, javascript, header and footer for UCSC's LibApps.

## Updating CSS

Styles come from the Library's drupal theme, Spencer. 
Stlyes are maintained and should be copied from the global CSS file at:
/sites/all/themes/spencer/css/global.css

## Updating Javascript

Javsacript also comes from the Spencer theme. It can be found at
/sites/all/themes/spencer/js/spencer.js

Note that most of the code there is legacy and is not copied here.

## Updating the header

To update the header, look at the source code of the main website. Copy
from the `<!-- Header -->` tag down to the closing div just before the
`<!-- Page -->` tag.

## Updating the footer

Each Libapp has a separate footer to include the specific login link.
Changes to the global footer should be carefully reproduced on each separate
file.