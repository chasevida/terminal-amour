# iTerm
iTerm is a replacement for the standard Terminal that comes with your Mac and is packed with additional features and capabilities. It's free too!

* [iTerm download](https://www.iterm2.com/)

## Theme
The default theme in my opinion is a little unhelpful. Luckily there are tons out there. The one I'm currently using is [Teerb](Teerb.itermcolors). I'm also using a nice font [SourceCode Pro](https://github.com/adobe-fonts/source-code-pro).

To install the theme save [Teerb](Teerb.itermcolors) somewhere on your computer. Open iTerm preferences and under the profiles tab you can create a new default profile. Once you've done this select the *colors* tab and at the bottom of this you can see a select box *Load presets*. Using this you can import the Teerb theme. Once you've imported it you will need to use the select box again to actually select the theme.

Ensure you set your new profile as default.

### Fonts
From the same panel in the preferences (see above) you can go to the *text* tab to select the fonts you'd like to use.

### Font Glyphs
It's handy to have a set of Non-ASCII font glyphs that can be used within terminal and Vim. I'd recomend the [powerline fonts](https://github.com/powerline/fonts).

To install these you will need to perform the following:

	$ cd ~/
	$ git clone https://github.com/powerline/fonts.git
	$ ./fonts/install.sh
	$ rm -rf fonts
	
**Please Note** this is assuming you do not have a folder already called *fonts* in your home directory.