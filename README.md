# Fastub-Advance
An advance version of fastub API mocking client supporting 

It's based on base code created by github user @prabjot678.

This one supports dynamic responses, by using expressions 
to place data from request.

The format is as below:
$ - represents root
. - accessing next level of hierarchy.

For example, if you want to access 
firstname from request, i.e {name:{firstName:"a", lastName:"b"}}
Use below expression as value inside double quotes

{$.name.firstName}
This will fetch data from request and put it in the response.

Sample response:

{nameRes:"{$.name.firstName}"}

