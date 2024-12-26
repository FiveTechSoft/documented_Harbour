### Alphabetically Ordered Table of C Functions in `src/vm/eval.c`

| Function Name          | Parameters                                              | Return Value | Description |
|------------------------|---------------------------------------------------------|--------------|-------------|
| `hb_evalBlock`         | `PHB_ITEM pCodeBlock, ...`                              | `void`       | Evaluates a code block with a variable number of parameters. |
| `hb_evalBlock0`        | `PHB_ITEM pCodeBlock`                                   | `void`       | Evaluates a code block with no parameters. |
| `hb_evalBlock1`        | `PHB_ITEM pCodeBlock, PHB_ITEM pParam`                  | `void`       | Evaluates a code block with one parameter. |
| `hb_evalLaunch`        | `PHB_EVALINFO pEvalInfo`                                | `PHB_ITEM`   | Launches the evaluation of an item or symbol. |
| `hb_evalNew`           | `PHB_EVALINFO pEvalInfo, PHB_ITEM pItem`                | `HB_BOOL`    | Initializes the evaluation info structure with an item. |
| `hb_evalPutParam`      | `PHB_EVALINFO pEvalInfo, PHB_ITEM pItem`                | `HB_BOOL`    | Adds a parameter to the evaluation info structure. |
| `hb_evalRelease`       | `PHB_EVALINFO pEvalInfo`                                | `HB_BOOL`    | Releases the parameters stored in the evaluation info structure. |
| `hb_execFromArray`     | `PHB_ITEM pParam`                                       | `HB_BOOL`    | Executes a function or code block from an array of parameters. |
| `hb_itemDo`            | `PHB_ITEM pItem, HB_ULONG ulPCount, ...`                | `PHB_ITEM`   | Executes a function or code block with a variable number of parameters. |
| `hb_itemDoC`           | `const char* szFunc, HB_ULONG ulPCount, ...`            | `PHB_ITEM`   | Executes a function by name with a variable number of parameters. |
| `HB_FUNC( HB_EXECFROMARRAY )` | None                                                      | `void`       | Executes a function or code block from an array of parameters. |
| `HB_FUNC( HB_EXECMSG )`       | None                                                      | `void`       | Executes a function with an object as the `SELF` value. |
| `HB_FUNC( HB_FORNEXT )`       | None                                                      | `void`       | Executes a code block in a loop with a start, end, and optional step value. |
