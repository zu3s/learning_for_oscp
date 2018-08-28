# Command Substitution and Constants
Now, we will add a timestamp to the page to indicate when it was last updated.
add`<p>Updated on $(date +"%x %r %Z") by $USER</p>` below the h1 tag.

The characters "$()" tell the shell, "substitute the results of the enclosed command." 
The *date* command has many features and formatting options. To look at them all, try this:
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzM3MDA0NzA3LC00MTAwMzQ1MTFdfQ==
-->