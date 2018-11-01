# Flatbuffers Compatible Table

| parent | table | struct | union | vector | string | enum | scalar |
| ------ | ----- | ------ | ----- | ------ | ------ | ---- | ------ |
| root   | Y     | Y      |       |        |        |      |        |
| table  | Y     | Y      | Y     | Y      | Y      | Y    | Y      |
| struct |       | Y      |       |        |        | Y    | Y      |
| union  | Y     | Y      |       |        |        |      |        |
| vector | Y     | Y      | Y     |        | Y      | Y    | Y      |

If there is a `Y` in row A column B, B can be used as a child of A. If it is
blank, B is not allowed as a child of A.

Parent `root` means which type can be used as a root object.
