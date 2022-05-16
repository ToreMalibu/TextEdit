# TextEdit
<h3>Simple but useful Text Editor</h3>
This was built because of all of the trouble I saw on StackOverflow and gitHub making a simple text editor work.<br /><br />
The main theme of peeps trying to make a text editor is the use of string.replace()
The problem with string.replace is this: If you want to bold the word "the" in the fourth paragraph. There's a good chance that the word "the" 
occurs many times before the one you want to bold. String.replace will replace the first instance of the word "the". Not the one you highlighted/selected.<br /><br />
<b>The solution: Break up everything in the textarea/editor into three variables.</b> <br />
1) The string you want to replace<br /> 
2) Everything before your selection<br />
3) Everything after your selection.<br /><br />
Now we DO use string.replace() on the selected text to add formatting. Last we concatenate (before, str.replace, after) and dump the result into a div
so you can confirm that the formatting you wanted acutually worked!<br /><br />
No need for adding HTML BRs. Line breaks / hard returns (\r, \n) are replaced with HTML BRs when the resulting text is displayed.
