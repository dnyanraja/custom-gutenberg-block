# custom-gutenberg-block
WP Plugin to create custom gutenberg block

What is gutenberg?
“Gutenberg” is the codename for the new WordPress editor focus. The goal of this focus is to create a new post and page editing experience that makes it easy for anyone to create rich post layouts.

In coming days wordpress will incorporate the gutenberg editor into its core and now, all the designers and developer needs to start getting used to this editor.

At the core of Gutenberg lies the concept of the block. A post in Gutenberg is then a collection of blocks.


#1 Create a main plugin file index.php
Define plugin name, author, URI, Version etc.

#2 Write hook to include editor assets
// Hook: Editor assets.
add_action( 'enqueue_block_editor_assets', 'gb_block_basic_editor_assets' );

#3 Write function to include editor assets 
Function gb_block_basic_editor_assets()

#4  Write hook to include frontend assets
//Hook: Frontend assets.
add_action( 'enqueue_block_assets', 'gb_block_basic_block_assets' );

#5 Write function to include frontend assets 
Function gb_block_basic_block_assets()

#6 Main code of the block resided within the js file called block.js, you can name it anything you wish.
block.js

#7 Block Js contains "Immediately Invoked Function Expressions" IIFE 

