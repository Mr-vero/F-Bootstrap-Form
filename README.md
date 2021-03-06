### PHP Bootstrap Form helper 4.0 (previously [PFBC/PHP Form Builder Class](http://code.google.com/p/php-form-builder-class/))

[Documentation](http://smarttechdo.com/~avb/pfbc/) :: [Discussions](http://groups.google.com/d/forum/php-form-builder-class) :: [Issues](https://github.com/avbdr/php-bootstrap-form/issues)

[Elements Demo](http://smarttechdo.com/~avb/pfbc/example.php) :: [Source Code](https://github.com/avbdr/php-bootstrap-form/blob/master/example.php)

[Bootstrap4 Elements Demo](http://smarttechdo.com/~avb/pfbc/example.php?v=4) :: [Source Code](http://smarttechdo.com/~avb/pfbc/example.php)

Latest Features:

1. Bootstrap 3 and 4 support
2. Added new simple API. Old API is still supported
3. Added 'shared' element property to share 1 row between multiple elements in SideBySide View
4. View class renamed to FormView class
5. Added Form::renderArray() helper function
6. Fixed prepend and append properties handling
7. Added icon property to buttons

New API:
```php
Form::open ("login");
echo '<legend>Login</legend>';
Form::Hidden ("id");
Form::Email ("Email Address:", "email", array("required" => 1));
Form::Password ("Password:", "password", array("required" => 1));
Form::Checkbox ("", "remember", array("1" => "Remember me"));
Form::Button ("Login");
Form::Button ("Cancel", "button", array("onclick" => "history.go(-1);"));
Form::close ();
```
