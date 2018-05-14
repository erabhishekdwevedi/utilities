
# Common String Handling Code Snippets


* Compares String
```
Boolean message = myString.equals(yourString);
Boolean message = myString.equalsIgnoreCase(yourString); 
```

* If String(myString) contains money it will return true
```
Boolean message = myString.contains("money");
```

*Removes space from front and end of String.
```
String newString = oldString.trim());
```


* Replace All Occurrence of ABC to XYZ in a string
```
String newString = oldString.replace("ABC","XYZ");
```

* Removes All Extra Characters except A-Z and 0-9 
```
String newString = oldString.replaceAll("[^A-Za-z0-9]","");

```

* Remove Spaces from String

```
String newString=oldString.replaceAll("\\s+","");

```

* Get first word of a paragraph
```
String word = paragraph.split("\\s",0)[0]);
```
