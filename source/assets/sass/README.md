## CSS Structure is based on the Drupal Omega Theme file structure mainly because it makes the most sense to me. 

Thanks to Fred Parke's for writing the best blog post I could find that explaines a good SASS file struction. Its a great read: http://www.fredparke.com/blog/get-aquainted-omegas-sass-file-structure

SASS file roadmap
sass/              
|
|- abstractions/             # Partials for custom mixins and extends.
|              
|- base/                     # Partials for base styles of raw HTML elements.
|  |-- _forms.scss           
|  |-- _lists.scss           
|  ...
|
|- components/               # Partials for individual components of your site.
|  |-- _navigation.scss      
|  |-- _search.scss          
|  ...
|
|- variables/                # Partials for sass variables.
|  |-- _colors.scss          
|  |-- _typography.scss      
|  ...
|
|- themename.hacks.scss      # Can be used for temporary hot-fixes.
|- themename.no-query.scss   # Re-renders themename.styles.scss without any media queries.
|- themename.normalize.scss  # Provides CSS reset based on the legacy variables.
|- themename.styles.scss     # Primary stylesheet aggregates the partials into a single file. 


The import process
The themename.styles.scss file first imports the external libraries and then imports our partials.

@import "compass";
@import "breakpoint";
@import "singularitygs";
@import "toolkit-no-css";

@import "variables/**/*";
@import "abstractions/**/*";
@import "base/**/*";
@import "components/**/*";

The variables folder is imported first, and for good reason - all of your other sass files will likely need to access these variables.

You can see from the asterisks that sass globbing is being used - this is really handy, it means the sass files inside these folders (and any subfolders within them) will automatically be imported.
