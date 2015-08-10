<strong>"Unexpected {".</strong> If you are getting an "unexpected {" error when you activate OpenBook, it is because you have an earlier version of PHP. Your server must support at least PHP 5. Note: my server was set to PHP4, but upgrading to PHP5 was a <a href='http://support.netfirms.com/article.php?id=713'>simple switch</a>.

<strong>No book data for this book number.</strong> The default booknumber type is ISBN. OpenBook also supports other types like the Open Library key, the 'number' that starts with "OL". Using the Visual Editor dialogue, note the different booknumber types in the drop-down and the prefixes added to the booknumber when you insert them in a post. You can manually add these prefixes if you wish.

<strong>Blank post.</strong> If you are using OpenBook and nothing is happening, e.g., blank post, it is likely that a PHP error is occuring due to a missing requirement, but that WordPress is suppressing the error. For troubleshooting, enable error reporting. See this <a href='http://forums.westhost.com/showthread.php?t=10186'>thread</a>.

<strong>Strange formatting.</strong> If you using OpenBook and getting strange formatting results, it is possible that your theme or other plugins have a conflict with OpenBook. Test switching your theme and disabling other plugins, enabling them one at a time.

<strong>Visual Editor button fails to open form.</strong> I experienced this problem on my production WordPress server when I was using Internet Explorer 8. I resolved it by clicking IE8's "Compatibility View" button.

<strong>ISBN with an "X" in it</strong>. Some ISBNs at Open Library have a non-standard "X" in them, and do not return data. Use the Open Library ID instead. The bug has been brought to the attention of Open Library.

<strong>Error message saying that curl must be enabled.</strong> You get this message when you activate OpenBook and the curl library has not been enabled on your web server. If you have just installed XAMPP, find your php.ini file and uncomment the line: extension=php\_curl.dll. Restart Apache.

Also see this <a href='http://code.google.com/p/openbook4wordpress/wiki/pluginrequirements'>plugin requirement information</a>.