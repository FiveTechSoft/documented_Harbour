### Alphabetically Ordered Table of C Functions in `src/vm/extend.c`

| Function Name               | Parameters                                                     | Return Value                                            | Description |
|-----------------------------|----------------------------------------------------------------|---------------------------------------------------------|-------------|
| `hb_extIsArray`             | `int iParam`                                                   | `HB_BOOL`: `TRUE` if the item is an array, `FALSE` otherwise | Detects if the extend system is using an array item |
| `hb_extIsNil`               | `int iParam`                                                   | `HB_BOOL`: `TRUE` if the item is `NIL`, `FALSE` otherwise | Checks if the item is `NIL` |
| `hb_extIsObject`            | `int iParam`                                                   | `HB_BOOL`: `TRUE` if the item is an object, `FALSE` otherwise | Detects if the extend system is using an object item |
| `hb_param`                  | `int iParam, long lMask`                                       | `PHB_ITEM`: Pointer to the parameter item or `NULL` if not found or masked | Retrieves a parameter item with a specified mask |
| `hb_paramError`             | `int iParam`                                                   | `PHB_ITEM`: Pointer to the parameter item or a static NIL item if not found | Retrieves a parameter item, returning a static NIL item if not found |
| `hb_parinfo`                | `int iParam`                                                   | `HB_ULONG`: Type information of the parameter | Retrieves type information of a parameter |
| `hb_parinfa`                | `int iParamNum, HB_SIZE nArrayIndex`                           | `HB_SIZE`: Length of the array or type of the array element | Retrieves array information of a parameter |
| `hb_parc`                   | `int iParam`                                                   | `const char *`: Pointer to the string value or `NULL` if not found | Retrieves a string parameter |
| `hb_parcx`                  | `int iParam`                                                   | `const char *`: Pointer to the string value or an empty string if not found | Retrieves a string parameter, returning an empty string if not found |
| `hb_parclen`                | `int iParam`                                                   | `HB_SIZE`: Length of the string parameter | Retrieves the length of a string parameter |
| `hb_parcsiz`                | `int iParam`                                                   | `HB_SIZE`: Length of the string parameter including the terminating zero byte | Retrieves the length of a string parameter including the terminating zero byte |
| `hb_pards`                  | `int iParam`                                                   | `const char *`: Date string in YYYYMMDD format | Retrieves a date parameter as a string |
| `hb_pardsbuff`              | `char * szDate, int iParam`                                    | `char *`: Pointer to the date string buffer | Retrieves a date parameter as a string into a buffer |
| `hb_pardl`                  | `int iParam`                                                   | `long`: Julian date number | Retrieves a date parameter as a Julian date number |
| `hb_partd`                  | `int iParam`                                                   | `double`: Timestamp value | Retrieves a date and time parameter as a timestamp value |
| `hb_partdt`                 | `long * plJulian, long * plMilliSec, int iParam`               | `HB_BOOL`: `TRUE` if the parameter is a valid datetime, `FALSE` otherwise | Retrieves a date and time parameter as Julian date and milliseconds |
| `hb_parl`                   | `int iParam`                                                   | `int`: Logical value (1 for `TRUE`, 0 for `FALSE`) | Retrieves a logical parameter |
| `hb_parldef`                | `int iParam, int iDefValue`                                    | `int`: Logical value (1 for `TRUE`, 0 for `FALSE`) or default value if not found | Retrieves a logical parameter with a default value |
| `hb_parnd`                  | `int iParam`                                                   | `double`: Numeric value | Retrieves a numeric parameter |
| `hb_parni`                  | `int iParam`                                                   | `int`: Integer value | Retrieves an integer parameter |
| `hb_parnidef`               | `int iParam, int iDefValue`                                    | `int`: Integer value or default value if not found | Retrieves an integer parameter with a default value |
| `hb_parnl`                  | `int iParam`                                                   | `long`: Long integer value | Retrieves a long integer parameter |
| `hb_parnldef`               | `int iParam, long lDefValue`                                   | `long`: Long integer value or default value if not found | Retrieves a long integer parameter with a default value |
| `hb_parns`                  | `int iParam`                                                   | `HB_ISIZ`: Size value | Retrieves a size parameter |
| `hb_parnsdef`               | `int iParam, HB_ISIZ nDefValue`                                | `HB_ISIZ`: Size value or default value if not found | Retrieves a size parameter with a default value |
| `hb_parnll`                 | `int iParam`                                                   | `HB_LONGLONG`: Long long integer value | Retrieves a long long integer parameter |
| `hb_parnint`                | `int iParam`                                                   | `HB_MAXINT`: Maximum integer value | Retrieves a maximum integer parameter |
| `hb_parnintdef`             | `int iParam, HB_MAXINT nDefValue`                              | `HB_MAXINT`: Maximum integer value or default value if not found | Retrieves a maximum integer parameter with a default value |
| `hb_parptr`                 | `int iParam`                                                   | `void *`: Pointer value | Retrieves a pointer parameter |
| `hb_parptrGC`               | `const HB_GC_FUNCS * pFuncs, int iParam`                       | `void *`: Pointer value managed by garbage collector | Retrieves a garbage collector-managed pointer parameter |
| `hb_parvc`                  | `int iParam, ...`                                              | `const char *`: Pointer to the string value or `NULL` if not found | Retrieves a string parameter with optional array index |
| `hb_parvcx`                 | `int iParam, ...`                                              | `const char *`: Pointer to the string value or an empty string if not found | Retrieves a string parameter with optional array index, returning an empty string if not found |
| `hb_parvclen`               | `int iParam, ...`                                              | `HB_SIZE`: Length of the string parameter | Retrieves the length of a string parameter with optional array index |
| `hb_parvcsiz`               | `int iParam, ...`                                              | `HB_SIZE`: Length of the string parameter including the terminating zero byte | Retrieves the length of a string parameter with optional array index, including the terminating zero byte |
| `hb_parvds`                 | `int iParam, ...`                                              | `const char *`: Date string in YYYYMMDD format | Retrieves a date parameter as a string with optional array index |
| `hb_parvdsbuff`             | `char * szDate, int iParam, ...`                               | `char *`: Pointer to the date string buffer | Retrieves a date parameter as a string into a buffer with optional array index |
| `hb_parvdl`                 | `int iParam, ...`                                              | `long`: Julian date number | Retrieves a date parameter as a Julian date number with optional array index |
| `hb_parvtd`                 | `int iParam, ...`                                              | `double`: Timestamp value | Retrieves a date and time parameter as a timestamp value with optional array index |
| `hb_parvtdt`                | `long * plJulian, long * plMilliSec, int iParam, ...`          | `HB_BOOL`: `TRUE` if the parameter is a valid datetime, `FALSE` otherwise | Retrieves a date and time parameter as Julian date and milliseconds with optional array index |
| `hb_parvl`                  | `int iParam, ...`                                              | `int`: Logical value (1 for `TRUE`, 0 for `FALSE`) | Retrieves a logical parameter with optional array index |
| `hb_parvnd`                 | `int iParam, ...`                                              | `double`: Numeric value | Retrieves a numeric parameter with optional array index |
| `hb_parvni`                 | `int iParam, ...`                                              | `int`: Integer value | Retrieves an integer parameter with optional array index |
| `hb_parvnl`                 | `int iParam, ...`                                              | `long`: Long integer value | Retrieves a long integer parameter with optional array index |
| `hb_parvns`                 | `int iParam, ...`                                              | `HB_ISIZ`: Size value | Retrieves a size parameter with optional array index |
| `hb_parvnll`                | `int iParam, ...`                                              | `HB_LONGLONG`: Long long integer value | Retrieves a long long integer parameter with optional array index |
| `hb_parvnint`               | `int iParam, ...`                                              | `HB_MAXINT`: Maximum integer value | Retrieves a maximum integer parameter with optional array index |
| `hb_parvptr`                | `int iParam, ...`                                              | `void *`: Pointer value | Retrieves a pointer parameter with optional array index |
| `hb_parvptrGC`              | `const HB_GC_FUNCS * pFuncs, int iParam, ...`                  | `void *`: Pointer value managed by garbage collector | Retrieves a garbage collector-managed pointer parameter with optional array index |
| `hb_pcount`                 | None                                                           | `int`: Number of parameters passed to the function | Retrieves the number of parameters passed to the function |
| `hb_ret`                    | None                                                           | `void`                                                  | Clears the return item |
| `hb_reta`                   | `HB_SIZE nLen`                                                 | `void`                                                  | Creates a new array as the return item |
| `hb_retc`                   | `const char * szText`                                          | `void`                                                  | Returns a string parameter |
| `hb_retc_null`              | None                                                           | `void`                                                  | Returns a `NULL` string parameter |
| `hb_retc_buffer`            | `char * szText`                                                | `void`                                                  | Returns a string parameter, taking ownership of the buffer |
| `hb_retc_const`             | `const char * szText`                                          | `void`                                                  | Returns a constant string parameter |
| `hb_retclen`                | `const char * szText, HB_SIZE nLen`                            | `void`                                                  | Returns a string parameter with a specified length |
| `hb_retclen_buffer`         | `char * szText, HB_SIZE nLen`                                  | `void`                                                  | Returns a string parameter with a specified length, taking ownership of the buffer |
| `hb_retclen_const`          | `const char * szText, HB_SIZE nLen`                            | `void`                                                  | Returns a constant string parameter with a specified length |
| `hb_retds`                  | `const char * szDate`                                          | `void`                                                  | Returns a date parameter as a string |
| `hb_retd`                   | `int iYear, int iMonth, int iDay`                              | `void`                                                  | Returns a date parameter |
| `hb_retdl`                  | `long lJulian`                                                 | `void`                                                  | Returns a date parameter as a Julian date number |
| `hb_rettd`                  | `double dTimeStamp`                                            | `void`                                                  | Returns a timestamp parameter |
| `hb_rettdt`                 | `long lJulian, long lMilliSec`                                 | `void`                                                  | Returns a date and time parameter as Julian date and milliseconds |
| `hb_retl`                   | `int iLogical`                                                 | `void`                                                  | Returns a logical parameter |
| `hb_retnd`                  | `double dNumber`                                               | `void`                                                  | Returns a numeric parameter |
| `hb_retni`                  | `int iNumber`                                                  | `void`                                                  | Returns an integer parameter |
| `hb_retnl`                  | `long lNumber`                                                 | `void`                                                  | Returns a long integer parameter |
| `hb_retns`                  | `HB_ISIZ nNumber`                                              | `void`                                                  | Returns a size parameter |
| `hb_retnll`                 | `HB_LONGLONG llNumber`                                         | `void`                                                  | Returns a long long integer parameter |
| `hb_retnint`                | `HB_MAXINT nNumber`                                            | `void`                                                  | Returns a maximum integer parameter |
| `hb_retnlen`                | `double dNumber, int iWidth, int iDec`                         | `void`                                                  | Returns a numeric parameter with specified width and decimals |
| `hb_retndlen`               | `double dNumber, int iWidth, int iDec`                         | `void`                                                  | Returns a numeric parameter with specified width and decimals |
| `hb_retnilen`               | `int iNumber, int iWidth`                                      | `void`                                                  | Returns an integer parameter with specified width |
| `hb_retnllen`               | `long lNumber, int iWidth`                                     | `void`                                                  | Returns a long integer parameter with specified width |
| `hb_retnlllen`              | `HB_LONGLONG llNumber, int iWidth`                             | `void`                                                  | Returns a long long integer parameter with specified width |
| `hb_retnintlen`             | `HB_MAXINT nNumber, int iWidth`                                | `void`                                                  | Returns a maximum integer parameter with specified width |
| `hb_retptr`                 | `void * pointer`                                               | `void`                                                  | Returns a pointer parameter |
| `hb_retptrGC`               | `void * pointer`                                               | `void`                                                  | Returns a garbage collector-managed pointer parameter |
| `hb_stor`                   | `int iParam`                                                   | `int`: 1 on success, 0 on failure | Clears a parameter item |
| `hb_storc`                  | `const char * szText, int iParam`                              | `int`: 1 on success, 0 on failure | Stores a string parameter |
| `hb_storclen`               | `const char * szText, HB_SIZE nLen, int iParam`                | `int`: 1 on success, 0 on failure | Stores a string parameter with a specified length |
| `hb_storclen_buffer`        | `char * szText, HB_SIZE nLen, int iParam`                      | `int`: 1 on success, 0 on failure | Stores a string parameter with a specified length, taking ownership of the buffer |
| `hb_stords`                 | `const char * szDate, int iParam`                              | `int`: 1 on success, 0 on failure | Stores a date parameter as a string |
| `hb_stordl`                 | `long lJulian, int iParam`                                     | `int`: 1 on success, 0 on failure | Stores a date parameter as a Julian date number |
| `hb_stortd`                 | `double dTimeStamp, int iParam`                                | `int`: 1 on success, 0 on failure | Stores a timestamp parameter |
| `hb_stortdt`                | `long lJulian, long lMilliSec, int iParam`                     | `int`: 1 on success, 0 on failure | Stores a date and time parameter as Julian date and milliseconds |
| `hb_storl`                  | `int iLogical, int iParam`                                     | `int`: 1 on success, 0 on failure | Stores a logical parameter |
| `hb_storni`                 | `int iValue, int iParam`                                       | `int`: 1 on success, 0 on failure | Stores an integer parameter |
| `hb_stornl`                 | `long lValue, int iParam`                                      | `int`: 1 on success, 0 on failure | Stores a long integer parameter |
| `hb_storns`                 | `HB_ISIZ nValue, int iParam`                                   | `int`: 1 on success, 0 on failure | Stores a size parameter |
| `hb_stornll`                | `HB_LONGLONG llValue, int iParam`                              | `int`: 1 on success, 0 on failure | Stores a long long integer parameter |
| `hb_stornint`               | `HB_MAXINT nValue, int iParam`                                 | `int`: 1 on success, 0 on failure | Stores a maximum integer parameter |
| `hb_stornd`                 | `double dNumber, int iParam`                                   | `int`: 1 on success, 0 on failure | Stores a numeric parameter |
| `hb_storptr`                | `void * pointer, int iParam`                                   | `int`: 1 on success, 0 on failure | Stores a pointer parameter |
| `hb_storptrGC`              | `void * pointer, int iParam`                                   | `int`: 1 on success, 0 on failure | Stores a garbage collector-managed pointer parameter |
| `hb_storvc`                 | `const char * szText, int iParam, ...`                         | `int`: 1 on success, 0 on failure | Stores a string parameter with optional array index |
| `hb_storvclen`              | `const char * szText, HB_SIZE nLen, int iParam, ...`           | `int`: 1 on success, 0 on failure | Stores a string parameter with a specified length and optional array index |
| `hb_storvclen_buffer`       | `char * szText, HB_SIZE nLen, int iParam, ...`                 | `int`: 1 on success, 0 on failure | Stores a string parameter with a specified length and optional array index, taking ownership of the buffer |
| `hb_storvds`                | `const char * szDate, int iParam, ...`                         | `int`: 1 on success, 0 on failure | Stores a date parameter as a string with optional array index |
| `hb_storvdl`                | `long lJulian, int iParam, ...`                                | `int`: 1 on success, 0 on failure | Stores a date parameter as a Julian date number with optional array index |
| `hb_storvtd`                | `double dTimeStamp, int iParam, ...`                           | `int`: 1 on success, 0 on failure | Stores a timestamp parameter with optional array index |
| `hb_storvtdt`               | `long lJulian, long lMilliSec, int iParam, ...`                | `int`: 1 on success, 0 on failure | Stores a date and time parameter as Julian date and milliseconds with optional array index |
| `hb_storvl`                 | `int iLogical, int iParam, ...`                                | `int`: 1 on success, 0 on failure | Stores a logical parameter with optional array index |
| `hb_storvni`                | `int iValue, int iParam, ...`                                  | `int`: 1 if successful, 0 otherwise                     | Stores an integer value in a specified parameter or array element. |
| `hb_storvnl`                | `long lValue, int iParam, ...`                                 | `int`: 1 if successful, 0 otherwise                     | Stores a long value in a specified parameter or array element. |
| `hb_storvns`                | `HB_ISIZ nValue, int iParam, ...`                              | `int`: 1 if successful, 0 otherwise                     | Stores a size integer value in a specified parameter or array element. |
| `hb_storvnll`               | `HB_LONGLONG llValue, int iParam, ...`                         | `int`: 1 if successful, 0 otherwise                     | Stores a long long value in a specified parameter or array element. |
| `hb_storvnint`              | `HB_MAXINT nValue, int iParam, ...`                            | `int`: 1 if successful, 0 otherwise                     | Stores a max integer value in a specified parameter or array element. |
| `hb_storvnd`                | `double dNumber, int iParam, ...`                              | `int`: 1 if successful, 0 otherwise                     | Stores a double value in a specified parameter or array element. |
| `hb_storvptr`               | `void * pointer, int iParam, ...`                              | `int`: 1 if successful, 0 otherwise                     | Stores a pointer value in a specified parameter or array element. |
| `hb_storvptrGC`             | `void * pointer, int iParam, ...`                              | `int`: 1 if successful, 0 otherwise                     | Stores a pointer value with garbage collection in a specified parameter or array element. |
| `hb_pcount`                 | None                                                           | `int`: Number of parameters passed to the function      | Returns the number of parameters passed to the function. |
