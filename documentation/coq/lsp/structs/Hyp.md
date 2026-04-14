# `Hyp`

Abstraction of a Coq hypothesis.

## Attributes

`names : List[str]`
> Contains the names of the hypothesis.

`ty : str`
> The type of the hypothesis.

`definition : Optional[str]`
> The body of the hypothesis.


## Operations

```python
Hyp(self, names: List[str], ty: str, definition: Optional[str])
```
> Creates a new Hyp object.
> 
> `names : List[str]`
> >  The names of the hypothesis.
> 
> `ty : str`
> > The type of the hypothesis.
> 
> `definition : Optional[str]`
> > The body of the hypothesis.