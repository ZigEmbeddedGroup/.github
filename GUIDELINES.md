# Zig Embedde Group Coding Guidelines

## Style Guide

ZEG uses the regular [Zig Style Guide](https://ziglang.org/documentation/master/#Style-Guide), but derives when it comes to function naming:

- Function in ZEG code are `snake_case`.

```zig
const namespace_name = @import("dir_name/file_name.zig");
const TypeName = @import("dir_name/TypeName.zig");
var global_var: i32 = undefined;
const const_name = 42;
const primitive_type_alias = f32;
const string_alias = []u8;

const StructName = struct {
    field: i32,
};
const StructAlias = StructName;

fn function_name(param_name: TypeName) void {
    var function_pointer = function_name;
    function_pointer();
    function_pointer = other_function;
    function_pointer();
}
const function_alias = function_name;

fn ListTemplateFunction(comptime ChildType: type, comptime fixed_size: usize) type {
    return List(ChildType, fixed_size);
}

fn ShortList(comptime T: type, comptime n: usize) type {
    return struct {
        field_name: [n]T,
        fn methodName() void {}
    };
}

// The word XML loses its casing when used in Zig identifiers.
const xml_document =
    \\<?xml version="1.0" encoding="UTF-8"?>
    \\<document>
    \\</document>
;
const XmlParser = struct {
    field: i32,
};

// The initials BE (Big Endian) are just another word in Zig identifier names.
fn read_u32_be() u32 {}
```

## Terminology

There's a lot of words out there, and sometimes precise and uniform language helps communicating.

The following table contains words we should try to use when referring to certain things or actions.

| Explanation                                                                                                                        | Primary Term | Accepted Alternative | Don't use |
| ---------------------------------------------------------------------------------------------------------------------------------- | ------------ | -------------------- | --------- |
| Continuous sequence of bytes without an inherent delimiter. It doesn't matter if you write 10, then 20 bytes or 20, then 10 bytes. | Stream       |                      |           |
| A known-length sequence of bytes with well defined boundaries. Not necessarily fixed size.                                         | Datagram     | Packet               |           |
| A piece of known-length data without well defined boundaries                                                                       | Chunk        |                      |           |
| Data is inserted into a continous stream.                                                                                          | write        |                      |           |
| Data is extracted from a contious stream.                                                                                          | read         |                      |           |
| Data is transmitted as a single datagram.                                                                                          | send         |                      |           |
| Data is received as a single datagram.                                                                                             | receive      |                      |           |
| The action of setting the level of a GPIO pin.                                                                                     | set          |                      | write     |
| The action of reading the level from a GPIO pin.                                                                                   | get          |                      | read      |
