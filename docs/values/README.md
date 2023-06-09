# Примитивные типы данных

| Тип            |   Эквивалент в С   | Описание                                                     |
|----------------|:------------------:|--------------------------------------------------------------|
| i8             | int8_t             | Знаковый 8-ми битный integer                                 |
| u8             | uint8_t            | Положительный 8-ми битный integer                            |
| i16            | int16_t            | Знаковый 16-ти битный integer                                |
| u16            | uint16_t           | Положительный 16-ти битный integer                           |
| i32            | int32_t            | Знаковый 32-х битный integer                                 |
| u32            | uint32_t           | Положительный 32-х битный integer                            |
| i64            | int64_t            | Знаковый 64-х битный integer                                 |
| u64            | uint64_t           | Положительный 64-х битный integer                            |
| i128           | __int128           | Знаковый 128-ми битный integer                               |
| u128           | unsigned __int128  | Положительный 128-ми битный integer                          |
| isize          | intptr_t           | Знаковый integer размером с указатель                        |
| usize          | uintptr_t, size_t  | Положительный integer размером с указатель                   |
| c_short        | short              | Для ABI совместимости с C                                    |
| c_ushort       | unsigned short     | Для ABI совместимости с C                                    |
| c_int          | int                | Для ABI совместимости с C                                    |
| c_uint         | unsigned int       | Для ABI совместимости с C                                    |
| c_long         | long               | Для ABI совместимости с C                                    |
| c_ulong        | unsigned long      | Для ABI совместимости с C                                    |
| c_longlong     | long long          | Для ABI совместимости с C                                    |
| c_ulonglong    | unsigned long long | Для ABI совместимости с C                                    |
| c_longdouble   | long double        | Для ABI совместимости с C                                    |
| f16            | _Float16           | 16-ти битный float (10-ти битная мантисса)                   |
| f32            | float              | 32-х битный float (23-х битная мантисса)                     |
| f64            | double             | 64-х битный float (52-х битная мантисса)                     |
| f80            | double             | 80-ти битный float (64-х битная мантисса)                    |
| f128           | _Float128          | 128-ми битный float (112-ти битная мантисса)                 |
| bool           | bool               | true или false                                               |
| anyopaque      | void               | Используется для указателей со стертым типом                 |
| void           | -                  | Void                                                         |
| noreturn       | -                  | Тип break, continue, return, unreachable and while (true) {} |
| type           | -                  | Тип типов (родительский тип)                                 |
| anyerror       | -                  | Ошибки                                                       |
| comptime_int   | -                  | Только integer значения, известные во время компиляции       |
| comptime_float | -                  | Только float значения, известные во время компиляции         |

``` zig
pub fn main() void {
    const integer: i64 = 123;
    const fnumber: f64 = 0.54;
}
```

## Примитивные значения

| Имя          |                             Описание                             |
|--------------|:----------------------------------------------------------------:|
| true и false | Булевые значения                                                 |
| null         | Используется для назначения переменной с опциональным типом null |
| undefined    | Используется для переменных без значения                         |

``` zig
const isOk: bool = true; 
```
