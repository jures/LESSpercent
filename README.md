# LESS script to convert px values to percentages
The script uses Namespaces for the most common CSS rules which are needed when styling a responsive webpage with percentages.

Inspired by the following blog post: http://www.ifdattic.com/2011/10/19/converting-px-to-ems-with-less/

# Author
Jure Stern - [Follow me on Twitter](https://twitter.com/JureStern)

# How to use it
Download the **pxtofluid.less** file and @import it into your main stylesheet file. If you changed the default font size change the value in the @basefont variable:

	//Size of your font, without px.
	@basefont: 16;

After that you can use the following for your CSS rules:

	// Calculating the font size and line-height
	#pxtofluid > .font-size( @basefont, 16 );
  #pxtofluid > .line-height( 21, @basefont );

	// First is your desired value, second is the value of the parent element
	#pxtofluid > .width( 500, 1000 );
	#pxtofluid > .height( 500, 1000 );
	#pxtofluid > .padding( 20, 1000 );
	#pxtofluid > .margin( 20, 1000 );
 	#pxtofluid > .margin-top( 20, 1000 );
 	#pxtofluid > .margin-right( 20, 1000 );
 	#pxtofluid > .margin-bottom( 20, 1000 );
 	#pxtofluid > .margin-left( 20, 1000 );
 	#pxtofluid > .padding-top( 20, 1000 );
 	#pxtofluid > .padding-right( 20, 1000 );
 	#pxtofluid > .padding-bottom( 20, 1000 );
 	#pxtofluid > .padding-left( 20, 1000 );

# TODO
* Combining the CSS rules for padding and margin to use the shorthand version.