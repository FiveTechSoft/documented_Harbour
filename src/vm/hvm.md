# HVM Functions Documentation

| Function Name | Signature | Parameters | Description | Return Value |
|---------------|-----------|------------|-------------|--------------|
| `hb_vmAddInt` | `static void hb_vmAddInt( PHB_ITEM pResult, HB_LONG lAdd )` | `pResult`: Item to which the integer is added. <br> `lAdd`: Integer to add. | Adds an integer to a given item. | None |
| `hb_vmAddModuleFunction` | `static void hb_vmAddModuleFunction( PHB_FUNC_LIST * pLstPtr, HB_INIT_FUNC pFunc, void * cargo )` | `pLstPtr`: Pointer to the function list. <br> `pFunc`: Function to add. <br> `cargo`: Additional data. | Adds a module function to the function list. | None |
| `hb_vmAnd` | `static void hb_vmAnd( void )` | None | Performs logical AND on the top two values of the stack and replaces them with the result. | None |
| `hb_vmArrayDim` | `static void hb_vmArrayDim( HB_USHORT uiDimensions )` | `uiDimensions`: Number of dimensions. | Generates an array with the specified number of dimensions and initializes those dimensions from the stack values. | None |
| `hb_vmArrayGen` | `static void hb_vmArrayGen( HB_SIZE nElements )` | `nElements`: Number of elements. | Generates an array with the specified number of elements and fills it from the stack values. | None |
| `hb_vmArrayItemPop` | `static void hb_vmArrayItemPop( HB_SIZE nIndex )` | `nIndex`: Index of the item to pop. | Pops an item from the array. | None |
| `hb_vmArrayItemPush` | `static void hb_vmArrayItemPush( HB_SIZE nIndex )` | `nIndex`: Index of the item to push. | Pushes an item to the array. | None |
| `hb_vmArrayNew` | `static HB_BOOL hb_vmArrayNew( PHB_ITEM pArray, HB_USHORT uiDimension )` | `pArray`: The array item. <br> `uiDimension`: Number of dimensions. | Creates a new array with the specified number of dimensions. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_vmArrayPop` | `static void hb_vmArrayPop( void )` | None | Pops a value from the stack. | None |
| `hb_vmArrayPush` | `static void hb_vmArrayPush( void )` | None | Pushes an array element to the stack, removing the array and the index from the stack. | None |
| `hb_vmArrayPushRef` | `static void hb_vmArrayPushRef( void )` | None | Pushes a reference to an array element to the stack, removing the array and the index from the stack. | None |
| `hb_vmCalcIntWidth` | `static int hb_vmCalcIntWidth( HB_MAXINT nNumber )` | `nNumber`: The integer number. | Calculates the width of an integer. | Returns the width of the integer. |
| `hb_vmCleanModuleFunctions` | `static void hb_vmCleanModuleFunctions( void )` | None | Cleans up module functions. | None |
| `hb_vmDebugEntry` | `static void hb_vmDebugEntry( int nMode, int nLine, const char * szName, int nIndex, PHB_ITEM pFrame )` | `nMode`: Debug mode. <br> `nLine`: Line number. <br> `szName`: Name of the module. <br> `nIndex`: Index. <br> `pFrame`: Frame item. | Enters the debugger at a specific point. | None |
| `hb_vmDebuggerEndProc` | `static void hb_vmDebuggerEndProc( void )` | None | Notifies the debugger for an endproc. | None |
| `hb_vmDebuggerExit` | `static void hb_vmDebuggerExit( HB_BOOL fRemove )` | `fRemove`: Flag to remove. | Shuts down the debugger. | None |
| `hb_vmDebuggerShowLine` | `static void hb_vmDebuggerShowLine( HB_USHORT uiLine )` | `uiLine`: Line number. | Makes the debugger show a specific source code line. | None |
| `hb_vmDivide` | `static void hb_vmDivide( PHB_ITEM pResult, PHB_ITEM pItem1, PHB_ITEM pItem2 )` | `pResult`: Result item. <br> `pItem1`: First item. <br> `pItem2`: Second item. | Divides the given values. | None |
| `hb_vmDoBlock` | `static HARBOUR hb_vmDoBlock( void )` | None | Executes a codeblock. | Returns the result of the codeblock execution. |
| `hb_vmDoExitFunctions` | `static void hb_vmDoExitFunctions( void )` | None | Executes all defined PRGs EXIT functions. | None |
| `hb_vmDoInitFunctions` | `static void hb_vmDoInitFunctions( HB_BOOL fClipInit )` | `fClipInit`: Flag for clip initialization. | Executes all defined PRGs INIT functions. | None |
| `hb_vmDoInitHVM` | `static void hb_vmDoInitHVM( void )` | None | Initializes the Harbour Virtual Machine. | None |
| `hb_vmDoInitHelp` | `static void hb_vmDoInitHelp( void )` | None | Initializes the help system. | None |
| `hb_vmDoInitStatics` | `static void hb_vmDoInitStatics( void )` | None | Executes all _INITSTATICS functions. | None |
| `hb_vmDoModuleExitFunctions` | `static void hb_vmDoModuleExitFunctions( void )` | None | Executes module exit functions. | None |
| `hb_vmDoModuleFunctions` | `static void hb_vmDoModuleFunctions( PHB_FUNC_LIST * pLstPtr )` | `pLstPtr`: Pointer to the function list. | Executes module functions. | None |
| `hb_vmDoModuleInitFunctions` | `static void hb_vmDoModuleInitFunctions( void )` | None | Executes module initialization functions. | None |
| `hb_vmDoModuleLibFunctions` | `static void hb_vmDoModuleLibFunctions( PHB_FUNC_LIST * pLstPtr, void * hDynLib )` | `pLstPtr`: Pointer to the function list. <br> `hDynLib`: Dynamic library handle. | Executes module library functions. | None |
| `hb_vmDoModuleQuitFunctions` | `static void hb_vmDoModuleQuitFunctions( void )` | None | Executes module quit functions. | None |
| `hb_vmDoModuleSetLibID` | `static void hb_vmDoModuleSetLibID( PHB_FUNC_LIST pLst, void * hDynLib, void * hNewDynLib )` | `pLst`: Function list. <br> `hDynLib`: Dynamic library handle. <br> `hNewDynLib`: New dynamic library handle. | Sets the library ID for a module. | None |
| `hb_vmDuplUnRef` | `static void hb_vmDuplUnRef( void )` | None | Duplicates the latest value on the stack and unrefs the source one. | None |
| `hb_vmDuplicate` | `static void hb_vmDuplicate( void )` | None | Duplicates the latest value on the stack. | None |
| `hb_vmEqual` | `static void hb_vmEqual( void )` | None | Checks if the two latest values on the stack are equal, removes both and leaves the result. | None |
| `hb_vmExactlyEqual` | `static void hb_vmExactlyEqual( void )` | None | Checks if the two latest values on the stack are exactly equal, removes both and leaves the result. | None |
| `hb_vmForTest` | `static void hb_vmForTest( void )` | None | Tests for the end condition of a `for` loop. | None |
| `hb_vmFrame` | `static void hb_vmFrame( HB_USHORT usLocals, unsigned char ucParams )` | `usLocals`: Number of local variables. <br> `ucParams`: Number of parameters. | Increases the stack pointer for the amount of locals and params supplied. | None |
| `hb_vmFuncPtr` | `static void hb_vmFuncPtr( void )` | None | Pushes a function address pointer and removes the symbol from the stack. | None |
| `hb_vmGreater` | `static void hb_vmGreater( void )` | None | Checks if the latest - 1 value is greater than the latest, removes both and leaves the result. | None |
| `hb_vmGreaterEqual` | `static void hb_vmGreaterEqual( void )` | None | Checks if the latest - 1 value is greater than or equal to the latest, removes both and leaves the result. | None |
| `hb_vmHashGen` | `static void hb_vmHashGen( HB_SIZE nElements )` | `nElements`: Number of elements. | Generates a hash with the specified number of elements and fills it from the stack values. | None |
| `hb_vmInc` | `static void hb_vmInc( PHB_ITEM pItem )` | `pItem`: The item to increment. | Increments the latest numeric value on the stack. | None |
| `hb_vmInstring` | `static void hb_vmInstring( void )` | None | Checks whether string 1 is contained in string 2. | None |
| `hb_vmItemRawRefCopy` | `static void hb_vmItemRawRefCopy( PHB_ITEM pDest )` | `pDest`: Destination item. | Copies a raw reference to an item. | None |
| `hb_vmItemRawRefDummy` | `static void hb_vmItemRawRefDummy( void * value )` | `value`: The value to reference. | Dummy function for item raw reference. | None |
| `hb_vmItemRawRefRead` | `static PHB_ITEM hb_vmItemRawRefRead( PHB_ITEM pRefer )` | `pRefer`: Reference item. | Reads a raw reference from an item. | Returns the item. |
| `hb_vmItemRawRefWrite` | `static PHB_ITEM hb_vmItemRawRefWrite( PHB_ITEM pRefer, PHB_ITEM pSource )` | `pRefer`: Reference item. <br> `pSource`: Source item. | Writes a raw reference to an item. | Returns the reference item. |
| `hb_vmItemRefClear` | `static void hb_vmItemRefClear( void * value )` | `value`: The value to clear. | Clears an item reference. | None |
| `hb_vmItemRefCopy` | `static void hb_vmItemRefCopy( PHB_ITEM pDest )` | `pDest`: Destination item. | Copies an item reference. | None |
| `hb_vmItemRefMark` | `static void hb_vmItemRefMark( void * value )` | `value`: The value to mark. | Marks an item reference for garbage collection. | None |
| `hb_vmItemRefRead` | `static PHB_ITEM hb_vmItemRefRead( PHB_ITEM pRefer )` | `pRefer`: Reference item. | Reads a reference from an item. | Returns the item. |
| `hb_vmItemRefWrite` | `static PHB_ITEM hb_vmItemRefWrite( PHB_ITEM pRefer, PHB_ITEM pSource )` | `pRefer`: Reference item. <br> `pSource`: Source item. | Writes a reference to an item. | Returns the reference item. |
| `hb_vmLess` | `static void hb_vmLess( void )` | None | Checks if the latest - 1 value is less than the latest, removes both and leaves the result. | None |
| `hb_vmLessEqual` | `static void hb_vmLessEqual( void )` | None | Checks if the latest - 1 value is less than or equal to the latest, removes both and leaves the result. | None |
| `hb_vmLocalName` | `static void hb_vmLocalName( HB_USHORT uiLocal, const char * szLocalName )` | `uiLocal`: Local variable index. <br> `szLocalName`: Local variable name. | Provides locals and parameters index and name information for the debugger. | None |
| `hb_vmMacroArrayGen` | `static void hb_vmMacroArrayGen( HB_USHORT uiArgSets )` | `uiArgSets`: Number of argument sets. | Generates an array from arguments set on the HVM stack. | None |
| `hb_vmMacroDo` | `static void hb_vmMacroDo( HB_USHORT uiArgSets )` | `uiArgSets`: Number of argument sets. | Executes a function passing arguments set on the HVM stack. | None |
| `hb_vmMacroFunc` | `static void hb_vmMacroFunc( HB_USHORT uiArgSets )` | `uiArgSets`: Number of argument sets. | Executes a procedure passing arguments set on the HVM stack. | None |
| `hb_vmMacroPushIndex` | `static void hb_vmMacroPushIndex( void )` | None | Pushes a macro array index. | None |
| `hb_vmMacroSend` | `static void hb_vmMacroSend( HB_USHORT uiArgSets )` | `uiArgSets`: Number of argument sets. | Executes a procedure passing arguments set on the HVM stack. | None |
| `hb_vmMinus` | `static void hb_vmMinus( PHB_ITEM pResult, PHB_ITEM pItem1, PHB_ITEM pItem2 )` | `pResult`: Result item. <br> `pItem1`: First item. <br> `pItem2`: Second item. | Subtracts the given values. | None |
| `hb_vmModulus` | `static void hb_vmModulus( PHB_ITEM pResult, PHB_ITEM pItem1, PHB_ITEM pItem2 )` | `pResult`: Result item. <br> `pItem1`: First item. <br> `pItem2`: Second item. | Calculates the modulus of the given values. | None |
| `hb_vmModuleName` | `static void hb_vmModuleName( const char * szModuleName )` | `szModuleName`: Module name. | Provides PRG and function name information for the debugger. | None |
| `hb_vmMult` | `static void hb_vmMult( PHB_ITEM pResult, PHB_ITEM pItem1, PHB_ITEM pItem2 )` | `pResult`: Result item. <br> `pItem1`: First item. <br> `pItem2`: Second item. | Multiplies the given values. | None |
| `hb_vmNegate` | `static void hb_vmNegate( void )` | None | Negates the latest value on the stack. | None |
| `hb_vmNot` | `static void hb_vmNot( void )` | None | Changes the latest logical value on the stack. | None |
| `hb_vmNotEqual` | `static void hb_vmNotEqual( void )` | None | Checks if the two latest values on the stack are not equal, removes both and leaves the result. | None |
| `hb_vmOr` | `static void hb_vmOr( void )` | None | Performs logical OR on the latest two values, removes them and leaves the result on the stack. | None |
| `hb_vmPlus` | `static void hb_vmPlus( PHB_ITEM pResult, PHB_ITEM pItem1, PHB_ITEM pItem2 )` | `pResult`: Result item. <br> `pItem1`: First item. <br> `pItem2`: Second item. | Sums the given values. | None |
| `hb_vmPopAlias` | `static void hb_vmPopAlias( void )` | None | Pops the workarea number from the eval stack. | None |
| `hb_vmPopAliasedField` | `static void hb_vmPopAliasedField( PHB_SYMB pSym )` | `pSym`: Aliased field symbol. | Pops an aliased field from the eval stack. | None |
| `hb_vmPopAliasedVar` | `static void hb_vmPopAliasedVar( PHB_SYMB pSym )` | `pSym`: Aliased variable symbol. | Pops an aliased variable from the eval stack. | None |
| `hb_vmPopLocal` | `static void hb_vmPopLocal( int iLocal )` | `iLocal`: Local variable index. | Pops the stack's latest value onto a local variable. | None |
| `hb_vmPopLogical` | `static HB_BOOL hb_vmPopLogical( void )` | None | Pops the stack's latest value and returns its logical value. | Returns the logical value of the popped item. |
| `hb_vmPopStatic` | `static void hb_vmPopStatic( HB_USHORT uiStatic )` | `uiStatic`: Static variable index. | Pops the stack's latest value onto a static variable. | None |
| `hb_vmPower` | `static void hb_vmPower( PHB_ITEM pResult, PHB_ITEM pItem1, PHB_ITEM pItem2 )` | `pResult`: Result item. <br> `pItem1`: First item. <br> `pItem2`: Second item. | Raises the first value to the power of the second value. | None |
| `hb_vmPushAParams` | `static void hb_vmPushAParams( void )` | None | Pushes array items. | None |
| `hb_vmPushAlias` | `static void hb_vmPushAlias( void )` | None | Pushes the current workarea number. | None |
| `hb_vmPushAliasedField` | `static void hb_vmPushAliasedField( PHB_SYMB pSym )` | `pSym`: Aliased field symbol. | Pushes an aliased field onto the eval stack. | None |
| `hb_vmPushAliasedVar` | `static void hb_vmPushAliasedVar( PHB_SYMB pSym )` | `pSym`: Aliased variable symbol. | Pushes an aliased variable onto the eval stack. | None |
| `hb_vmPushBlock` | `static void hb_vmPushBlock( const HB_BYTE * pCode, PHB_SYMB pSymbols, HB_SIZE nLen )` | `pCode`: Code block. <br> `pSymbols`: Symbols. <br> `nLen`: Length of the code block. | Creates a codeblock and pushes it onto the stack. | None |
| `hb_vmPushBlockShort` | `static void hb_vmPushBlock
