# F# RFC FS-NNNN - Compile Time Evaluation for Literals

The design suggestion [FILL ME IN](https://github.com/fsharp/fslang-suggestions/issues/fill-me-in) has been marked "approved in principle".

This RFC covers the detailed proposal for this suggestion.

- [x] [Suggestion](https://github.com/fsharp/fslang-suggestions/issues/FILL-ME-IN)
- [x] Approved in principle
- [ ] [Implementation](https://github.com/dotnet/fsharp/pull/FILL-ME-IN)
- [ ] Design Review Meeting(s) with @dsyme and others invitees
- [Discussion](https://github.com/fsharp/fslang-design/discussions/FILL-ME-IN)

# Summary

Allow to evaluate constants at compile time for literals.

# Motivation

At moment this gives compile time erro:

```
> [<Literal>]
- let four=2*2;;

  let four=2*2;;
  ---------^^^

/Users/adelar/stdin(12,10): error FS0267: Esta não é uma expressão constante ou um valor de atributo personalizado válido
```

# Detailed design

This is the bulk of the RFC. Explain the design in enough detail for somebody familiar
with the language to understand, and for somebody familiar with the compiler to implement.
This should get into specifics and corner-cases, and include examples of how the feature is used.

Example code:

```fsharp
let add x y = x + y
```

# Drawbacks

Why should we *not* do this?

# Alternatives

What other designs have been considered? What is the impact of not doing this?

# Compatibility

Please address all necessary compatibility questions:

* Is this a breaking change?
* What happens when previous versions of the F# compiler encounter this design addition as source code?
* What happens when previous versions of the F# compiler encounter this design addition in compiled binaries?
* If this is a change or extension to FSharp.Core, what happens when previous versions of the F# compiler encounter this construct?


# Unresolved questions

What parts of the design are still TBD?
