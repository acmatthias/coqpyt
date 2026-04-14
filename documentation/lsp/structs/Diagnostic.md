# `Diagnostic`

A structure representing a diagnostic about a part of a file. These can be anything from error, to warnings, to info, to hints.

## Attributes

`range : Range` [Range](./Range.md)
> The range at which the message applies in a resource file.

`severity : Optional[int]`
> The diagnostic's severity. The four allowed values are as follows:
> 1. Error
> 2. Warning
> 3. Information
> 4. Hint
> 
> If omitted it is up to the client to interpret diagnostics as error, warning, info or hint.

`code : Optional[str]`
> The diagnostic's code, which might appear in the user interface.

`source : Optional[str]`
> A human-readable string describing the source of this diagnostic, e.g. 'typescript' or 'super lint'.

`message : Optional[str]`
> The diagnostic's message.

`relatedInformation : Optional[List]`
> An array of related diagnostic information, e.g. when symbol-names within a scope collide all definitions can be marked via this property.


## Operations

```python
Diagnostic(self, range: Range | Dict, message: str, severity: Optional[int] = None, code: Optional[str] = None, codeDescription = None, source: Optional[str] = None, tags = None, relatedInformation: Optional[List] = None, data = None)
```
> Constructs a new Diagnostic instance.
> 
> `range : Range | Dict` [Range](./Range.md)
> > The range at which the message applies. If a dictionary is passed, it will be parsed to a Range.
> 
> `message : str`
> > The diagnostic's message.
> 
> `severity : Optional[int] = None`
> > *Optional.* The diagnostic's severity. Defaults to None.
> 
> `code : Optional[str] = None`
> > *Optional.* The diagnostic's code. Defaults to None.
> 
> `codeDescription = None`
> > *Optional.* Unused by CoqPyt. Defaults to None.
> 
> `source : Optional[str] = None`
> > *Optional.* A human-readable string describing the source of this diagnostic. Defaults to None.
> 
> `tags = None`
> > *Optional.* Unused by CoqPyt. Defaults to None.
> 
> `relatedInformation : Optional[List] = None`
> > *Optional.* An array of related diagnostic information. Defaults to None.
> 
> `data = None`
> > *Optional.* Unused by CoqPyt. Defaults to None.