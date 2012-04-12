# Wordpress Help Class #

### Description
This class can be used to create contextual help or insert a metabox containing help on various post types. The benefits of this class vs. using the basic Wordpress function is that it creates a page using another custom post type that can be edited using the standard Wordpress editor. This allows for easily updating the help vs. hard coding help. 

### Usage

This is not a plugin. To use this you must include this class in your plugin or theme and create the help by using the following code. 
Replace post and "Blog Post Help" with the appropriate post type. This will create a custom help box on the edit post screen.

    include 'wp-help-class/help-class.php';
	    $help = new wp_help();
	    $help->create_help(array('post_type' => 'post','page_title' => 'Blog Post Help'));

On the initial run of this function this will do the following things. 
- Create a new post type of help, assigning appropriate labels and other logical defaults
- Create a new post of the post type help with the title Blog Post Help and name of post_wp_help authored by the user with id 1
- Create a new metabox on the edit post screen with the title Help that displays the contents of the page titled post_wp_help
- Create a new contextual help tab on the edit post screen and display the contents of the page titled post_wp_help
 
### To Do

- Add ability to assign custom roles and make admins the default for editing help
- remove ability to publish the help post type
- error checking
- output validation for both metabox and contextual help tab
- stylesheet
