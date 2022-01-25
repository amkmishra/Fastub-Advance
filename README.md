# Fastub-Advance
An advance version of fastub API mocking client supporting.
Since file was more than 25MB had to split it in multiple files.
You can use 7zip to unzip it into one file, if you have a better place to keep it.
Do let me know in comments.

It's based on base code created by github user @prabjot678, it just adds support for dynamic response based on request data.
You can download original fastub jar at https://getfastub.com/
and source code from https://github.com/prabjot678/fastub.

This one supports dynamic responses, by using expressions 
to place data from request.

The format is as below:
$ - represents root
. - accessing next level of hierarchy.

For example, if you want to access 
firstname from request, i.e {name:{firstName:"a", lastName:"b"}}
Use below expression as value inside double quotes

{$.name.firstName}
This will fetch firstName (under name object) from request and put it in the response.

Sample response:

{nameRes:"{$.name.firstName}"}

