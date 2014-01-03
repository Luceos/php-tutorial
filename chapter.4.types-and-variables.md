# Types and variables
> We are not of the varying type

## Variables

The most powerful functionality of most programming language is the use of [variables](http://www.php.net/manual/en/language.variables.basics.php). Variables allow you to store a `value` which can be any type.

Variables are represented by a dollar sign `$` followed by the name of the variable. 

```php
$variableName		= 'The variable $variableName now contains this string as value';
var_dump( $variableName );
```

Variables are case sensitive and several theories exist in how we should name variables. My preference is to use [camelCase](http://en.wikipedia.org/wiki/CamelCase) as much as possible, where the first letter is lowercase and any new, seperate word gets an uppercase:

```php
$myProgress		= "50%";
var_dump( $myProgress );
$getGoing		= "yep, let's get going";
var_dump( $getGoing );
```
## Types

As said, variables are very powerful; you will be able to experience this for yourself with the following types.

> Please note the documentation about [types](http://www.php.net/manual/en/language.types.intro.php)

### String

As you've already seen, strings in PHP are used for texts. There are four official (also called native) ways of defining a string variable:

```php
$singleQuoted		= 'this is a single quoted string and will be parsed as is';
$doubleQuoted		= "this is a double quoted string, variables will be parsed, like this: $singleQuoted";
$hereDoc		= <<<<EOT
this is a heredoc string, variables will be parsed: $doubleQuoted
EOT;
$nowDoc			= <<<<'EOT'
this is a nowdoc string and will be parsed as is
EOT;

var_dump( $hereDoc );
var_dump( $nowDoc );
```

> In the above code example (also called [snippet](http://en.wikipedia.org/wiki/Snippet_(programming))) I didn't debug both `$singleQuoted` and `$doubleQuoted` variables on purpose. For both are included in the Heredoc string version. If you wish you can add your own debug for both variables to see what happens.

### Boolean

A boolean can be a value of either yes or no. These are represented by `TRUE` and `FALSE`; PHP allows you to write these case-insensitivily. Please use uppercase as the preferred naming convention.

Using booleans allows for checking whether something is true or false.

```php
$loggedIn		= TRUE;
var_dump( $loggedIn );
```

## Naming conventions

In this chapter I explained what the preferred naming convention is for types and variables. In no way do I demand you to follow them. However to increase readability and allow other developers to more easily use your code, I'd advise you to follow them.