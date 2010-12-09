# PHP-PS (Portable Shell)

PHP-PS is a portable PHP5 shell that can run chunks of PHP interactively.
A few others exist with more bash-like interaction, but they require PECL and
PHP extensions to be installed. This one will work anywhere.

Based on original script by:

	David Phillips <david@acz.org>
	http://david.acz.org/phpa/

The original script had a few errors, required [Readline PHP module](http://www.php.net/manual/en/book.readline.php),
would close on an empty line, didn't work with PHP 5.2+ and was missing a few
things but was a brilliant piece of code.

I have converted it to use a class simplify the "namespacing" of code. This
should avoid conflicts with the interactive code just as well as the original, but
be a lot more readable.


## Usage

	$ php pshell
	PHP 5.3.1 (cli) (Feb 11 2010 16:21:20) [Darwin]
	>>> 1+1
	2

## To-do

	1. Get it working nicely with more output types.
	2. Improve error handling.
	3. If possible support history on up. Probably not without some extensions.