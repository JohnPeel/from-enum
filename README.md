# from-enum

It has the same interface as thiserror's `#[from]` attribute, but it works in no-std.

## Example

```rust
use from_enum::From;

#[derive(From)]
enum MyEnum {
    String(#[from] String),
    Int(#[from] i32),
}
```
