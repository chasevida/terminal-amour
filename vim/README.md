# Vim
Vim is a test editor that comes with the default iTerm. It is incredibly powerful and useful in many situations where a traditional text editor may not be.

## Configuration
Vim can be configured with the use of a `.vimrc` file. This should live in your home directory. Lets create one if it does not already exist.

	$ cd ~/
	$ touch .vimrc
	
In this file we can now configure Vim however we like. I have an example configuration set up I use in the [vimrc.txt](vimrc.txt) file.

## Plugins/Extensions
Vim is highly customisable and comes with various package/module managers. A great place to check out available extensions is at [vimawesome.com](http://vimawesome.com/).

One of the many handy package managers is Vundle. At the top of the example [vimrc](vimrc.txt) file you will see a list of some helpful/cool vim extensions. To make the most of these we first need to instal [Vundle](https://github.com/gmarik/Vundle.vim).

### Installing Vundle
[Vundle](https://github.com/gmarik/Vundle.vim) offers a few options to install it and perhaps the simplest is a oneliner provided below.

	$ git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
	
Now that it's installed we can make the most of it by adding it's configuration to our `.vimrc` file. Again you can refer to their documentation or take a look at the example [vimrc](vimrc.txt) file I use.

## Vim Commands
Vim has so many commands it is overwhelming and quiet frankly a little difficult to use at first. I've added some real [basic command usage here](VIM-BASICS.md) to help you get started with it.