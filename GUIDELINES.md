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
