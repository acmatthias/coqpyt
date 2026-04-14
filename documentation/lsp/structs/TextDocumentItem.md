# `TextDocumentItem`

An item to transfer a text document from the client to the server.

## Attributes

`uri : str`
> The location of the file.

`languageId : str`
> Identifier of the file type. For a Coq file, this will be "coq".

`version : int`
> The version number of the file.

`text : str`
> The contents of the file.


## Operations

```python
TextDocumentItem(self, uri: str, languageId: str, version: int, text: str)
```
> Constructs a new Diagnostic instance.
> 
> `uri : str`
> > The location of the file.
> 
> `languageId : str`
> > Identifier of the file type. For a Coq file, this will be "coq".
> 
> `version : int`
> > The version number of the file.
> 
> `text : str`
> > The contents of the file.