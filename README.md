# README

## About

This is a pre commit script that checks added, copied, modified or renamed files for syntax errors and PSR2 coding standards.

## Installation

    # Put the pre-commit file in the .git/hooks/ folder in your git repository.
    https://raw.githubusercontent.com/Nebojsaa/phpCodingStandards/master/pre-commit 

    # create new hooks folder
    mkdir .git/hooks

    # move pre-commit to new hooks folder
	mv pre-commit .git/hooks/pre-commit

    # don't forget to make the pre-commit file executable
	chmod +x .git/hooks/pre-commit

## Usage

This will work automatically before every commit.


## Dependencies

### php codesniffer

[http://pear.php.net/package/PHP_CodeSniffer/redirected](http://pear.php.net/package/PHP_CodeSniffer/redirected)

You can install php codesniffer with these commands:

	sudo pear update-channels
	sudo pear install PHP_CodeSniffer
	
If you want to use it from your windows machine you should include into your composer phpcs like this.
    "require-dev": {
	"squizlabs/php_codesniffer": "2.*"	
	}

and everything will work automatically.
