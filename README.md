# ProcessWire Text Blocks Textformatter

This module enables you to assign a name to any block/region of text in a 
Textarea field. They are defined by typing `start_name` where you want the 
block to start, and `stop_name` where you want the block to stop. The 
block(s) of text can then be shown in any other Textarea field at runtime 
(site-wide) simply by typing the block name on its own line in the format 
`show_name`. Note that the word "name" in all of these examples would be 
wahtever you've decided to name the block. 

Released in 2017 as part of ProFields and released open source in 2024.  
License: MPL 2.0

## Introduction

For a full introduction to this module, use cases and examples, please see:
<https://processwire.com/blog/posts/text-blocks/>


## How to install and use

### Install

1. Copy all the files in this directory to:
   /site/modules/TextformatterTextBlocks/ 

2. In your admin, go to Modules > Refresh. 

3. Click the "Install" button next to Text Blocks. 

4. Determine which Textarea fields you want Text Blocks to be supported. 
   Locate those fields in Setup > Fields and edit them. The most likely 
   scenario is that you would apply it to your "body" field. When
   editing your field, go to the "Details" tab and select "Text Blocks"
   from the "Text formatters" select box. Save. 
   

### Test it out to make sure it is working

Edit any page that has a field using the Text Blocks text formatter. 
Define a block like this:
~~~~~
start_hello
   
Hello World!
   
stop_hello
~~~~~
Now go and edit another page that also has this field, and enter the 
following somewhere in the text:
~~~~~
show_hello
~~~~~
When viewing the page, you should see the "Hello World!" text.    