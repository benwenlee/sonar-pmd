# InsufficientStringBufferDeclaration
**Category:** `pmd`<br/>
**Rule Key:** `pmd:InsufficientStringBufferDeclaration`<br/>


-----

Failing to pre-size a StringBuffer properly could cause it to re-size many times during runtime. This rule checks the characters that are actually passed into StringBuffer.append(), but represents a best guess worst case scenario. An empty StringBuffer constructor initializes the object to 16 characters. This default is assumed if the length of the constructor can not be determined.
