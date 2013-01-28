vim-matnicer
============

Some conceal-based enhancements to matlab syntax. Beautify your code while making it a little bit less verbose.


Installation
------------

Put the folder `/after` in one of your run path folders, such as `~/.vim`. If you're using [pathogen](https://github.com/tpope/vim-pathogen) clone this project, [vundle](https://github.com/gmarik/vundle) users just add `Bundle  'capitancambio/vim-matnicer'` to your `.vimrc`.

Conceals 
--------

In order to activate the functionality just add the following lines to your `.vimrc`:


	"matnicer configuration
	au BufEnter *.m set conceallevel=2
	au BufEnter *.m set concealcursor=
	
or:

	au BufEnter *.m set conceallevel=2
	au BufEnter *.m set concealcursor=nc
	
Personally I find the behaviour of `nc` annoying so I leave it blank, check `:help concealcursor` for more info.


Greek letters
-------------

By default matnicer will process only matlab keywords ( function, end, ...), built-in functions (sum, mean , ...) and built-in constants ( pi, eps,...). You may find useful to coceal also greek letters if your algorithms use variables such as alpha or omega. To achieve this just set `g:matnicer_greek` to true in your `.vimrc`:

	let g:matnicer_greek=1

Screenshot
----------

 This how your code may look:

![Screenshot](http://github.com/capitancambio/vim-matnicer/raw/master/screenshot.png)

License
-------
"THE BEER-WARE LICENSE" (Revision 42):
<capitan.cambio@gmail.com> wrote this file. As long as you retain this notice you
can do whatever you want with this stuff. If we meet some day, and you think
this stuff is worth it, you can buy me a beer in return.





