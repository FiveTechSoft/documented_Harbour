### Alphabetically Ordered Table of C Functions in `src/vm/codebloc.c`

| Function Name               | Parameters                                                     | Return Value                                            | Description |
|-----------------------------|----------------------------------------------------------------|---------------------------------------------------------|-------------|
| `hb_codeblockGarbageDelete` | `void * Cargo`                                                 | `void`                                                  | Releases all allocated memory for the codeblock when called from the garbage collector. |
| `hb_codeblockGarbageMark`   | `void * Cargo`                                                 | `void`                                                  | Marks the codeblock for the garbage collector. |
| `hb_codeblockGetRef`        | `PHB_CODEBLOCK pCBlock, int iItemPos`                          | `PHB_ITEM`                                              | Gets a local variable passed by reference. |
| `hb_codeblockGetVar`        | `PHB_ITEM pItem, int iItemPos`                                 | `PHB_ITEM`                                              | Gets a local variable referenced in a codeblock. |
| `hb_codeblockId`            | `PHB_ITEM pItem`                                               | `void *`                                                | Retrieves the unique ID of the codeblock. |
| `hb_codeblockMacroNew`      | `const HB_BYTE * pBuffer, HB_SIZE nLen`                        | `PHB_CODEBLOCK`                                         | Creates a new macro-compiled codeblock. |
| `hb_codeblockNew`           | `const HB_BYTE * pBuffer, HB_USHORT uiLocals, const HB_BYTE * pLocalPosTable, PHB_SYMB pSymbols, HB_SIZE nLen` | `PHB_CODEBLOCK`                                         | Creates a new codeblock structure. |
| `hb_codeblockRefs`          | `PHB_ITEM pItem`                                               | `HB_COUNTER`                                            | Retrieves the number of references to the codeblock. |
