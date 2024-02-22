# JAVASCript Lecture 4
## Thema:String and Number
### 1.String:more than 9 methods
 ![подпись](https://i.imgur.com/20FIxbB.jpg)
## The at() method returns the character at a specified index (position) in a string.

## The at() method is supported in all modern browsers since March 2022:


## slice() extracts a part of a string and returns the extracted part in a new string.

## The method takes 2 parameters: start position, and end position (end not included) 
> In JavaScript, there are several methods that can be used to manipulate strings. Here are some of the most commonly used string methods in JavaScript:
- charAt(): This method returns the character at a specified index (position) in a string. .
- *charCodeAt(): This method returns the Unicode of the character at a specified index in a string*
- slice(): This method extracts a part of a string and returns the extracted part in a new string.
- substring(): This method extracts the characters from a string between two specified indices and returns the new sub-string
- toUpperCase(): This method converts a string to uppercase letters.
- toLowerCase(): This method converts a string to lowercase letters.
- concat(): This method joins two or more strings and returns a new joined string
- trim(): This method removes whitespace from both ends of a string
- 

 ![подпись](https://codedamn-blog.s3.amazonaws.com/wp-content/uploads/2022/08/21114451/js-number-methods.png)



## Converting to Upper and Lower Case
## A string is converted to upper case with toUpperCase():

## A string is converted to lower case with toLowerCase():

## JavaScript String toUpperCase()
## Example
## let text1 = "Hello World!";
## let text2 = text1.toUpperCase();
## JavaScript String toLowerCase()
## Example
## let text1 = "Hello World!";       // String
## let text2 = text1.toLowerCase();  // text2 is text1 converted to lower
## JavaScript String concat()
## concat() joins two or more strings:

## Example
## let text1 = "Hello";
## let text2 = "World";
## let text3 = text1.concat(" ", text2);
## The concat() method can be used instead of the plus operator. These two lines do the same:

## Example
## text = "Hello" + " " + "World!";
## text = "Hello".concat(" ", "World!");


![img](https://avatars.mds.yandex.net/i?id=45990688a2316fc37dbc0c2020703f5e4ba725fb-4825091-images-thumbs&n=13)
## Note that all comparison operators, including === and ==, compare strings case-sensitively. A common way to compare strings case-insensitively is to convert both to the same case (upper or lower) before comparing them.

## JS
## Copy to Clipboard
## function areEqualCaseInsensitive(str1, str2) {
 ##  return str1.toUpperCase() === str2.toUpperCase();
## }
## The choice of whether to transform by toUpperCase() or toLowerCase() is mostly arbitrary, and neither one is fully robust when extending beyond the Latin alphabet. For example, the German lowercase letter ß and ss are both transformed to SS by toUpperCase(), while the Turkish letter ı would be falsely reported as unequal to I by toLowerCase() unless specifically using toLocaleLowerCase("tr").
