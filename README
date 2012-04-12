# Wordpress Help Class #

### Description
This class can be used to create contextual help or insert a metabox containing help on various post types. The benefits of this class vs. using the basic Wordpress function is that it creates a page using another custom post type that can be edited using the standard Wordpress editor. This allows for easily updating the help vs. hard coding help. 

### Usage

This is not a plugin. To use this you must include this class in your plugin or theme and create the help by using the following code. 
Replace post and "Blog Post Help" with the appropriate post type. This will create a custom help box on the edit post screen.

    include 'wp-help-class/help-class.php';
	    $help = new wp_help();
	    $help->create_help(array('post_type' => 'post','page_title' => 'Blog Post Help'));

###To Do

- Add ability to assign custom roles and make admins the default for editing help
- remove ability to publish the help post type
- error checking
- output validation for both metabox and contextual help tab
- stylesheet
