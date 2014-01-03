# The first line
> Each step is a new one

## The root and the index file

On your local machine you now have a folder from which your site is served. This folder is called the root; originating from a tree's root.

In this root there might be a file called `index.html` or `index.php`; remove them and any other files. The index file is most commonly configured as the default file to be opened within a folder, like this:

`http://yourdomain.com` requests `/path/to/website/index.(html or php)`
`http://yourdomain.com/folder` requests `/path/to/website/folder/index.(html or php)`

## The PHP tags

Now create a file called `index.php` and open it in a text editor like notepad.

In order for the webserver to identify you are writing PHP you need to use opening and closing PHP tags:

`<?PHP` and `?>` everything between these tags is parsed by the webserver as PHP. Note that a closing tag is not necessary if it's also the end of the file.

So, let's try this on your site, in your `index.php` file write:

```php
<?PHP
```

Now open up your browser on [localhost](http://localhost) or [ipbased localhost](http://127.0.0.1) and see .. nothing! We've now only created an empty PHP file.

## Printing to the screen

There are several methods in PHP to output things to the screen. As said before, PHP in fact is not a markup language, so expect to use PHP essentially only for debugging when printing to the screen. Therefor we will now cover the most used debugging functions for PHP:

* `echo`
* `var_dump`

In your `index.php` edit your file to match the following:

```php
<?PHP
echo "Hello world";
```

When opening your browser to this page, you will see your first line of code; "Hello world". This classic example of a first line shows you how easy it is to create a web page. You could write all your websites using `echo` only. However that would be a waste of time and not very dynamic.

> From now on we will not show any PHP tags for opening or closing the document. So please make sure your document always starts with `<?PHP` when trying or writing code.

You now have witnessed how `echo` outputs a [`string`](http://www.php.net/manual/en/language.types.string.php) type to the screen. Strings represent text in PHP.

Another type is the [`array`](http://www.php.net/manual/en/language.types.array.php), which is a set of one of more items. For instance see the below array consisting of multiple strings:

```php
array( "this" , "is" , "an" , "array" );
```

If we would like to debug this array, we could use `var_dump`, a very nifty [function](http://www.php.net/manual/en/language.functions.php) to debug any type.

```php
var_dump( array( "this" , "is" , "an" , "array" ) );
```

The text now displaying in your browser shows you what the array is made up of.

Please note in both examples the PHP command ends with a `;`. This is necessary for all commands, except for the ones using `{` and `}` - more on these in the chapter about loops.