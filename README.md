# salesforce-developer-console-css-fix
This is a CSS fix for developer console themes.

I have noticed that on lover class monitors (the ones you get at work...), when you use dark themes (Help>Preferences), some highlighting makes code very unreadable. Namely, variable names are too dark on black baground and highlighting Visualforce text makes actual text unreadable.

Use Stylebot Chrome extension (or pack it as custom CSS) with this CSS:
<pre>
.CodeMirror-matchingbracket {
    background-color: #80E85C;
}
.CodeMirror-matchingtag {
    background: rgba(255,00,0,.3);
}
.VARIABLE_DECLARATION {
    color: #9B9BDA;
}
.VARIABLE_REFERENCE {
    color: #9B9BDA;
}
</pre>


Set the matching URL to `*.salesforce.com/_ui/common/apex/debug/ApexCSIPage`
