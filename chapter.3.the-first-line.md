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

