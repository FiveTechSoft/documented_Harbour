### Alphabetically Ordered Table of C Functions in src/vm/dynsym.c

| Function Name               | Parameters                                                     | Return Value                                            | Description |
|-----------------------------|----------------------------------------------------------------|---------------------------------------------------------|-------------|
| `hb_dynsymAreaHandle`       | `PHB_DYNS pDynSym`                                             | `int`: Area handle                                      | Retrieves the area handle associated with the dynamic symbol. |
| `hb_dynsymByItem`           | `PHB_ITEM pItem`                                               | `PHB_DYNS`: Pointer to dynamic symbol                   | Finds a dynamic symbol by an item. |
| `hb_dynsymCount`            | None                                                           | `HB_LONG`: Number of dynamic symbols                    | Returns the count of dynamic symbols. |
| `hb_dynsymEval`             | `PHB_DYNS_FUNC pFunction, void * Cargo`                        | `void`                                                  | Evaluates a function for each dynamic symbol. |
| `hb_dynsymFind`             | `const char * szName`                                          | `PHB_DYNS`: Pointer to dynamic symbol                   | Finds a dynamic symbol by name. |
| `hb_dynsymFindName`         | `const char * szName`                                          | `PHB_DYNS`: Pointer to dynamic symbol                   | Finds a dynamic symbol by its name, converting the name to uppercase. |
| `hb_dynsymFindSymbol`       | `const char * szName`                                          | `PHB_SYMB`: Pointer to symbol                           | Finds a symbol by name. |
| `hb_dynsymFromNum`          | `HB_SYMCNT uiSymNum`                                           | `PHB_DYNS`: Pointer to dynamic symbol                   | Gets a dynamic symbol from its number. |
| `hb_dynsymGet`              | `const char * szName`                                          | `PHB_DYNS`: Pointer to dynamic symbol                   | Finds or creates a dynamic symbol by name. |
| `hb_dynsymGetByIndex`       | `HB_LONG lIndex`                                               | `PHB_DYNS`: Pointer to dynamic symbol                   | Gets a dynamic symbol by its index. |
| `hb_dynsymGetCase`          | `const char * szName`                                          | `PHB_DYNS`: Pointer to dynamic symbol                   | Finds a dynamic symbol by name with case sensitivity. |
| `hb_dynsymGetMemvar`        | `PHB_DYNS pDynSym`                                             | `PHB_ITEM`: Memory variable                             | Gets the memory variable associated with the dynamic symbol. |
| `hb_dynsymGetSymbol`        | `const char * szName`                                          | `PHB_SYMB`: Pointer to symbol                           | Gets the symbol associated with a dynamic symbol. |
| `hb_dynsymInsert`           | `PHB_SYMB pSymbol, HB_SYMCNT uiPos`                            | `PHB_DYNS`: Pointer to dynamic symbol                   | Inserts a new dynamic symbol into the table. |
| `hb_dynsymIsFunction`       | `PHB_DYNS pDynSym`                                             | `HB_BOOL`: `TRUE` if it is a function                   | Checks if a dynamic symbol is a function. |
| `hb_dynsymIsMemvar`         | `PHB_DYNS pDynSym`                                             | `HB_BOOL`: `TRUE` if it is a memory variable            | Checks if a dynamic symbol is a memory variable. |
| `hb_dynsymName`             | `PHB_DYNS pDynSym`                                             | `const char *`: Name of the dynamic symbol              | Gets the name of a dynamic symbol. |
| `hb_dynsymNew`              | `PHB_SYMB pSymbol`                                             | `PHB_DYNS`: Pointer to dynamic symbol                   | Creates a new dynamic symbol. |
| `hb_dynsymPos`              | `const char * szName, HB_SYMCNT * puiPos`                      | `PHB_DYNS`: Pointer to dynamic symbol                   | Finds the position of a dynamic symbol or sets the position for insertion. |
| `hb_dynsymProtectEval`      | `PHB_DYNS_FUNC pFunction, void * Cargo`                        | `void`                                                  | Evaluates a function for each dynamic symbol in a protected manner. |
| `hb_dynsymRelease`          | None                                                           | `void`                                                  | Releases all dynamic symbols. |
| `hb_dynsymSetAreaHandle`    | `PHB_DYNS pDynSym, int iArea`                                  | `void`                                                  | Sets the area handle for a dynamic symbol. |
| `hb_dynsymSetMemvar`        | `PHB_DYNS pDynSym, PHB_ITEM pMemvar`                           | `void`                                                  | Sets the memory variable for a dynamic symbol. |
| `hb_dynsymSymbol`           | `PHB_DYNS pDynSym`                                             | `PHB_SYMB`: Pointer to symbol                           | Gets the symbol associated with a dynamic symbol. |
| `hb_dynsymToNum`            | `PHB_DYNS pDynSym`                                             | `HB_SYMCNT`: Symbol number                              | Converts a dynamic symbol to its number. |
| `hb_dynsymVerify`           | None                                                           | `int`: Result of verification                           | Verifies the integrity of dynamic symbols. |
| `hb_symbolAlloc`            | `const char * szName`                                          | `PHB_SYMB`: Pointer to symbol                           | Allocates a new symbol. |
| `hb_symbolNew`              | `const char * szName`                                          | `PHB_SYMB`: Pointer to symbol                           | Creates a new symbol. |
