# Привет, мир

[Пример](hello.zig) с официального сайта:

``` zig
const std = @import("std");

pub fn main() !void {
    const stdout = std.io.getStdOut().writer();
    try stdout.print("Привет, {s}!\n", .{"мир!"});
}
```
