# SimpleSyntax

This Sublime Text 3 package contains 4 simple syntax files. They only highlight and enable comments and is intended for use with configuration files. 

## Symbols

Another feature of **SimpleSyntax** is the possibility to add symbols/sections in your file. This is done by creating a comment where the first three characters are ` >>` followed by an optional string. Then you can use **Sublime Text's** built in function to *goto symbol* (default keybinding is: `ctrl+r`).

## Enabling the syntax

It is up to the user to enable the syntax, since many config files have the same name, but might have different comment types it is hard to do this *by filename*. Personally i use the package, [ApplySyntax](http://facelessuser.github.io/ApplySyntax/) with the following preferences:  

If installed manually:

``` json
"syntaxes": 
[
  {
    "syntax": "ssSemi/ssSemi",
    "rules": [{"contains": "syntax:ssSemi"} ]
  },
  {
    "syntax": "ssExcla/ssExcla",
    "rules": [{"contains": "syntax:ssExcla"} ]
  },
  {
    "syntax": "ssHash/ssHash",
    "rules": [{"contains": "syntax:ssHash"} ]
  },
  {
    "syntax": "ssDslash/ssDslash",
    "rules": [{"contains": "syntax:ssDslash"} ]
  }
]
```

If installed through package control:

``` json
"syntaxes": 
[
  {
    "syntax": "SimpleSyntax/ssSemi",
    "rules": [{"contains": "syntax:ssSemi"} ]
  },
  {
    "syntax": "SimpleSyntax/ssExcla",
    "rules": [{"contains": "syntax:ssExcla"} ]
  },
  {
    "syntax": "SimpleSyntax/ssHash",
    "rules": [{"contains": "syntax:ssHash"} ]
  },
  {
    "syntax": "SimpleSyntax/ssDslash",
    "rules": [{"contains": "syntax:ssDslash"} ]
  }
]
```

And a comment in the settings file that look something like this:  
`# syntax:ssHash`

## License

MIT License
