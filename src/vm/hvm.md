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
| `hb_vmPushBlockShort` | `static void hb_vmPushBlockShort( const HB_BYTE * pCode, PHB_SYMB pSymbols, HB_SIZE nLen )` | `pCode`: Pointer to the code block. <br> `pSymbols`: Pointer to the symbols. <br> `nLen`: Length of the code block. | Creates a code block. | None |
| `hb_vmPushDoubleConst` | `static void hb_vmPushDoubleConst( double dNumber, int iWidth, int iDec )` | `dNumber`: Double value to push. <br> `iWidth`: Width of the double value. <br> `iDec`: Number of decimal places. | Pushes a double constant onto the stack. | None |
| `hb_vmPushEvalSym` | `void hb_vmPushEvalSym( void )` | None | Pushes the evaluation symbol onto the stack. | None |
| `hb_vmPushFuncSymbol` | `void hb_vmPushFuncSymbol( PHB_SYMB pSym )` | `pSym`: Pointer to the function symbol. | Pushes a function symbol onto the stack. | None |
| `hb_vmPushIntegerConst` | `static void hb_vmPushIntegerConst( int iNumber )` | `iNumber`: Integer value to push. | Pushes an integer constant onto the stack. | None |
| `hb_vmPushItemRef` | `void hb_vmPushItemRef( PHB_ITEM pItem )` | `pItem`: Pointer to the item. | Pushes a reference to an item onto the stack. | None |
| `hb_vmPushLongConst` | `static void hb_vmPushLongConst( long lNumber )` | `lNumber`: Long value to push. | Pushes a long constant onto the stack. | None |
| `hb_vmPushMacroBlock` | `static void hb_vmPushMacroBlock( const HB_BYTE * pCode, HB_SIZE nSize, HB_USHORT usParams )` | `pCode`: Pointer to the code block. <br> `nSize`: Size of the code block. <br> `usParams`: Number of parameters. | Creates a macro-compiled code block. | None |
| `hb_vmPushObjectVarRef` | `static void hb_vmPushObjectVarRef( void )` | None | Pushes a reference to an object variable onto the stack. | None |
| `hb_vmPushStatic` | `static void hb_vmPushStatic( HB_USHORT uiStatic )` | `uiStatic`: Index of the static variable. | Pushes the content of a static variable onto the stack. | None |
| `hb_vmPushStaticByRef` | `static void hb_vmPushStaticByRef( HB_USHORT uiStatic )` | `uiStatic`: Index of the static variable. | Pushes a reference to a static variable onto the stack. | None |
| `hb_vmPushUnRef` | `static void hb_vmPushUnRef( void )` | None | Pushes the unreferenced latest value onto the stack. | None |
| `hb_vmPushVariable` | `static void hb_vmPushVariable( PHB_SYMB pVarSymb )` | `pVarSymb`: Pointer to the variable symbol. | Pushes an undeclared variable onto the stack. | None |
| `hb_vmReqEndProc` | `void hb_vmRequestEndProc( void )` | None | Requests the end of a procedure. | None |
| `hb_vmReqQuit` | `void hb_vmRequestQuit( void )` | None | Requests to quit the VM. | None |
| `hb_vmSeqBlock` | `static void hb_vmSeqBlock( void )` | None | Sets the begin sequence with a code block. | None |
| `hb_vmSetDynFunc` | `void hb_vmSetDynFunc( PHB_DYNS pDynSym )` | `pDynSym`: Pointer to the dynamic symbol. | Sets a dynamic function. | None |
| `hb_vmSetFunction` | `void hb_vmSetFunction( PHB_SYMB pOldSym, PHB_SYMB pNewSym )` | `pOldSym`: Pointer to the old symbol. <br> `pNewSym`: Pointer to the new symbol. | Sets a function symbol. | None |
| `hb_vmSetKeyPool` | `HB_BOOL hb_vmSetKeyPool( HB_BOOL fEnable )` | `fEnable`: Enable or disable the key pool. | Sets the key pool status. | Returns `HB_TRUE` if successful, `HB_FALSE` otherwise. |
| `hb_vmStaticsClear` | `static void hb_vmStaticsClear( void )` | None | Clears complex static variables. | None |
| `hb_vmStaticsRelease` | `static void hb_vmStaticsRelease( void )` | None | Releases arrays with static variables. | None |
| `hb_vmSuper` | `void hb_vmSuper( void )` | None | Calls a superclass method. | None |
| `hb_vmSwitch` | `static const HB_BYTE * hb_vmSwitch( const HB_BYTE * pCode, HB_USHORT casesCnt )` | `pCode`: Pointer to the code. <br> `casesCnt`: Number of cases. | Makes a switch statement. | Returns the pointer to the next code. |
| `hb_vmSwap` | `static void hb_vmSwap( int iCount )` | `iCount`: Number of items to swap. | Swaps items on the stack. | None |
| `hb_vmSwapAlias` | `static void hb_vmSwapAlias( void )` | None | Swaps items on the evaluation stack and pops the workarea number. | None |
| `hb_vmTSVarClean` | `static void hb_vmTSVarClean( void * pThreadItem )` | `pThreadItem`: Pointer to the thread item. | Cleans thread static variables. | None |
| `hb_vmTSVarMark` | `static void hb_vmTSVarMark( void * value )` | `value`: Value to mark. | Marks thread static variables. | None |
| `hb_vmTerminateThreads` | `void hb_vmTerminateThreads( void )` | None | Terminates all threads. | None |
| `hb_vmThreadInit` | `void hb_vmThreadInit( void * Cargo )` | `Cargo`: Pointer to the thread cargo. | Initializes a thread. | None |
| `hb_vmThreadIsMain` | `HB_BOOL hb_vmThreadIsMain( void * Cargo )` | `Cargo`: Pointer to the thread cargo. | Checks if the current thread is the main thread. | Returns `HB_TRUE` if it is the main thread, `HB_FALSE` otherwise. |
| `hb_vmThreadQuit` | `void hb_vmThreadQuit( void )` | None | Quits the current thread. | None |
| `hb_vmThreadRelease` | `void hb_vmThreadRelease( void * Cargo )` | `Cargo`: Pointer to the thread cargo. | Releases a thread. | None |
| `hb_vmThreadStart` | `PHB_ITEM hb_vmThreadStart( HB_ULONG ulAttr, PHB_CARGO_FUNC pFunc, void * cargo )` | `ulAttr`: Thread attributes. <br> `pFunc`: Pointer to the function to run. <br> `cargo`: Pointer to the thread cargo. | Starts a new thread. | Returns the thread item. |
| `hb_vmTryEval` | `HB_BOOL hb_vmTryEval( PHB_ITEM * pResult, PHB_ITEM pItem, HB_ULONG ulPCount, ... )` | `pResult`: Pointer to the result item. <br> `pItem`: Pointer to the item to evaluate. <br> `ulPCount`: Number of parameters. | Tries to evaluate an item. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_vmVFrame` | `static void hb_vmVFrame( HB_USHORT usLocals, unsigned char ucParams )` | `usLocals`: Number of local variables. <br> `ucParams`: Number of parameters. | Increases the stack pointer for the amount of locals and variable number of parameters supplied. | None |
| `hb_vmVerifyPCodeVersion` | `static void hb_vmVerifyPCodeVersion( const char * szModuleName, HB_USHORT uiPCodeVer )` | `szModuleName`: Name of the module. <br> `uiPCodeVer`: PCode version. | Verifies the PCode version. | None |
| `hb_xvmAddInt` | `HB_BOOL hb_xvmAddInt( HB_LONG lAdd )` | `lAdd`: Integer value to add. | Adds an integer to the stack. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmAlwaysBegin` | `HB_BOOL hb_xvmAlwaysBegin( void )` | None | Begins an always block. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmAlwaysEnd` | `HB_BOOL hb_xvmAlwaysEnd( void )` | None | Ends an always block. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmAnd` | `HB_BOOL hb_xvmAnd( void )` | None | Performs a logical AND operation. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmArrayDim` | `void hb_xvmArrayDim( HB_USHORT uiDimensions )` | `uiDimensions`: Number of dimensions. | Generates an array with the specified number of dimensions. | None |
| `hb_xvmArrayGen` | `void hb_xvmArrayGen( HB_SIZE nElements )` | `nElements`: Number of elements. | Generates an array and fills it with elements from the stack. | None |
| `hb_xvmArrayItemPop` | `HB_BOOL hb_xvmArrayItemPop( HB_SIZE nIndex )` | `nIndex`: Index of the array item. | Pops an array item. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmArrayItemPush` | `HB_BOOL hb_xvmArrayItemPush( HB_SIZE nIndex )` | `nIndex`: Index of the array item. | Pushes an array item. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmArrayPush` | `HB_BOOL hb_xvmArrayPush( void )` | None | Pushes an array element onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmArrayPushRef` | `HB_BOOL hb_xvmArrayPushRef( void )` | None | Pushes a reference to an array element onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmDivEq` | `HB_BOOL hb_xvmDivEq( void )` | None | Divides the top two stack elements and stores the result. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmDivEqPop` | `HB_BOOL hb_xvmDivEqPop( void )` | None | Divides and pops the stack elements. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmDivide` | `HB_BOOL hb_xvmDivide( void )` | None | Divides the top two stack elements. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmDivideByInt` | `HB_BOOL hb_xvmDivideByInt( HB_LONG lDivisor )` | `lDivisor`: Integer divisor. | Divides by an integer. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmDuplUnRef` | `void hb_xvmDuplUnRef( void )` | None | Duplicates and unreferences the top stack element. | None |
| `hb_xvmDuplicate` | `void hb_xvmDuplicate( void )` | None | Duplicates the top stack element. | None |
| `hb_xvmEqual` | `HB_BOOL hb_xvmEqual( void )` | None | Checks if the top two stack elements are equal. | Returns `HB_TRUE` if equal, `HB_FALSE` otherwise. |
| `hb_xvmEqualInt` | `HB_BOOL hb_xvmEqualInt( HB_LONG lValue )` | `lValue`: Integer value to compare. | Checks if the top stack element is equal to an integer. | Returns `HB_TRUE` if equal, `HB_FALSE` otherwise. |
| `hb_xvmEqualIntIs` | `HB_BOOL hb_xvmEqualIntIs( HB_LONG lValue, HB_BOOL * pfValue )` | `lValue`: Integer value to compare. <br> `pfValue`: Pointer to store the result. | Checks if the top stack element is equal to an integer and stores the result. | Returns `HB_TRUE` if equal, `HB_FALSE` otherwise. |
| `hb_xvmExactlyEqual` | `HB_BOOL hb_xvmExactlyEqual( void )` | None | Checks if the top two stack elements are exactly equal. | Returns `HB_TRUE` if exactly equal, `HB_FALSE` otherwise. |
| `hb_xvmExpEq` | `HB_BOOL hb_xvmExpEq( void )` | None | Exponentiates and stores the result. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmExpEqPop` | `HB_BOOL hb_xvmExpEqPop( void )` | None | Exponentiates and pops the stack elements. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmForTest` | `HB_BOOL hb_xvmForTest( void )` | None | Tests the end condition of a FOR loop. | Returns `HB_TRUE` if the end condition is met, `HB_FALSE` otherwise. |
| `hb_xvmFuncPtr` | `void hb_xvmFuncPtr( void )` | None | Pushes a function address pointer onto the stack. | None |
| `hb_xvmGreater` | `HB_BOOL hb_xvmGreater( void )` | None | Checks if the top stack element is greater than the next element. | Returns `HB_TRUE` if greater, `HB_FALSE` otherwise. |
| `hb_xvmGreaterEqual` | `HB_BOOL hb_xvmGreaterEqual( void )` | None | Checks if the top stack element is greater than or equal to the next element. | Returns `HB_TRUE` if greater or equal, `HB_FALSE` otherwise. |
| `hb_xvmGreaterEqualThenInt` | `HB_BOOL hb_xvmGreaterEqualThenInt( HB_LONG lValue )` | `lValue`: Integer value to compare. | Checks if the top stack element is greater than or equal to an integer. | Returns `HB_TRUE` if greater or equal, `HB_FALSE` otherwise. |
| `hb_xvmGreaterEqualThenIntIs` | `HB_BOOL hb_xvmGreaterEqualThenIntIs( HB_LONG lValue, HB_BOOL * pfValue )` | `lValue`: Integer value to compare. <br> `pfValue`: Pointer to store the result. | Checks if the top stack element is greater than or equal to an integer and stores the result. | Returns `HB_TRUE` if greater or equal, `HB_FALSE` otherwise. |
| `hb_xvmGreaterThenInt` | `HB_BOOL hb_xvmGreaterThenInt( HB_LONG lValue )` | `lValue`: Integer value to compare. | Checks if the top stack element is greater than an integer. | Returns `HB_TRUE` if greater, `HB_FALSE` otherwise. |
| `hb_xvmGreaterThenIntIs` | `HB_BOOL hb_xvmGreaterThenIntIs( HB_LONG lValue, HB_BOOL * pfValue )` | `lValue`: Integer value to compare. <br> `pfValue`: Pointer to store the result. | Checks if the top stack element is greater than an integer and stores the result. | Returns `HB_TRUE` if greater, `HB_FALSE` otherwise. |
| `hb_xvmInc` | `HB_BOOL hb_xvmInc( void )` | None | Increments the top stack element. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmIncEq` | `HB_BOOL hb_xvmIncEq( void )` | None | Increments and stores the result. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmIncEqPop` | `HB_BOOL hb_xvmIncEqPop( void )` | None | Increments and pops the stack elements. | Returns `HB_TRUE` on success, `HB_FALSE` otherwise. |
| `hb_xvmLess` | `HB_BOOL hb_xvmLess( void )` | None | Checks if the top stack element is less than the next element. | Returns `HB_TRUE` if less, `HB_FALSE` otherwise. |
| `hb_xvmLessEqual` | `HB_BOOL hb_xvmLessEqual( void )` | None | Checks if the top stack element is less than or equal to the next element. | Returns `HB_TRUE` if less or equal, `HB_FALSE` otherwise. |
| `hb_xvmLessEqualThenInt` | `HB_BOOL hb_xvmLessEqualThenInt( HB_LONG lValue )` | `lValue`: Integer value to compare. | Checks if the top stack element is less than or equal to an integer. | Returns `HB_TRUE` if less or equal, `HB_FALSE` otherwise. |
| `hb_xvmLessEqualThenIntIs` | `HB_BOOL hb_xvmLessEqualThenIntIs( HB_LONG lValue, HB_BOOL * pfValue )` | `lValue`: Integer value to compare. <br> `pfValue`: Pointer to store the result. | Checks if the top stack element is less than or equal to an integer and stores the result. | Returns `HB_TRUE` if less or equal, `HB_FALSE` otherwise. |
| `hb_xvmLessThenInt` | `HB_BOOL hb_xvmLessThenInt( HB_LONG lValue )` | `lValue`: Integer value to compare. | Checks if the top stack element is less than an integer. | Returns `HB_TRUE` if less, `HB_FALSE` otherwise. |
| `hb_xvmLessThenIntIs` | `HB_BOOL hb_xvmLessThenIntIs( HB_LONG lValue, HB_BOOL * pfValue )` | `lValue`: The integer value to compare. <br> `pfValue`: Pointer to store the result. | Checks if the latest value on the stack is less than the given integer and stores the result. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmLocalAdd` | `HB_BOOL hb_xvmLocalAdd( int iLocal )` | `iLocal`: The local variable index. | Adds the latest value on the stack to a local variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmLocalAddInt` | `HB_BOOL hb_xvmLocalAddInt( int iLocal, HB_LONG lAdd )` | `iLocal`: The local variable index. <br> `lAdd`: The integer value to add. | Adds an integer to a local variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmLocalDec` | `HB_BOOL hb_xvmLocalDec( int iLocal )` | `iLocal`: The local variable index. | Decrements the value of a local variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmLocalInc` | `HB_BOOL hb_xvmLocalInc( int iLocal )` | `iLocal`: The local variable index. | Increments the value of a local variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmLocalIncPush` | `HB_BOOL hb_xvmLocalIncPush( int iLocal )` | `iLocal`: The local variable index. | Increments the value of a local variable and pushes the result onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmLocalSetInt` | `void hb_xvmLocalSetInt( int iLocal, HB_LONG lValue )` | `iLocal`: The local variable index. <br> `lValue`: The integer value to set. | Sets the value of a local variable to an integer. | None |
| `hb_xvmMacroArrayGen` | `HB_BOOL hb_xvmMacroArrayGen( HB_USHORT uiArgSets )` | `uiArgSets`: The number of argument sets. | Generates an array from macro arguments. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMacroDo` | `HB_BOOL hb_xvmMacroDo( HB_USHORT uiArgSets )` | `uiArgSets`: The number of argument sets. | Executes a function passing arguments set on the HVM stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMacroFunc` | `HB_BOOL hb_xvmMacroFunc( HB_USHORT uiArgSets )` | `uiArgSets`: The number of argument sets. | Executes a procedure passing arguments set on the HVM stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMacroPush` | `HB_BOOL hb_xvmMacroPush( int iFlags )` | `iFlags`: Flags for the macro push. | Pushes a macro item onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMacroPushIndex` | `HB_BOOL hb_xvmMacroPushIndex( void )` | None | Pushes a macro array index onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMacroPushPare` | `HB_BOOL hb_xvmMacroPushPare( int iFlags )` | `iFlags`: Flags for the macro push. | Pushes a macro parenthesis item onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMacroSend` | `HB_BOOL hb_xvmMacroSend( HB_USHORT uiArgSets )` | `uiArgSets`: The number of argument sets. | Sends a macro-compiled message. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmModEq` | `HB_BOOL hb_xvmModEq( void )` | None | Performs modulus assignment on the top two stack values. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmModEqPop` | `HB_BOOL hb_xvmModEqPop( void )` | None | Performs modulus assignment and pops the result from the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmModulus` | `HB_BOOL hb_xvmModulus( void )` | None | Calculates the modulus of the top two stack values. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmModulusByInt` | `HB_BOOL hb_xvmModulusByInt( HB_LONG lDivisor )` | `lDivisor`: The divisor integer. | Calculates the modulus of the top stack value by an integer. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMult` | `HB_BOOL hb_xvmMult( void )` | None | Multiplies the top two stack values. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMultByInt` | `HB_BOOL hb_xvmMultByInt( HB_LONG lValue )` | `lValue`: The integer value to multiply. | Multiplies the top stack value by an integer. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMultEq` | `HB_BOOL hb_xvmMultEq( void )` | None | Performs multiplication assignment on the top two stack values. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmMultEqPop` | `HB_BOOL hb_xvmMultEqPop( void )` | None | Performs multiplication assignment and pops the result from the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmNegate` | `HB_BOOL hb_xvmNegate( void )` | None | Negates the top stack value. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmNot` | `HB_BOOL hb_xvmNot( void )` | None | Performs logical NOT on the top stack value. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmOr` | `HB_BOOL hb_xvmOr( void )` | None | Performs logical OR on the top two stack values. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPlus` | `HB_BOOL hb_xvmPlus( void )` | None | Adds the top two stack values. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPlusEq` | `HB_BOOL hb_xvmPlusEq( void )` | None | Performs addition assignment on the top two stack values. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPlusEqPop` | `HB_BOOL hb_xvmPlusEqPop( void )` | None | Performs addition assignment and pops the result from the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopAlias` | `HB_BOOL hb_xvmPopAlias( void )` | None | Pops the top stack value as an alias. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopAliasedField` | `HB_BOOL hb_xvmPopAliasedField( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the aliased field. | Pops the top stack value into an aliased field. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopAliasedFieldExt` | `HB_BOOL hb_xvmPopAliasedFieldExt( PHB_SYMB pAlias, PHB_SYMB pField )` | `pAlias`: The alias symbol. <br> `pField`: The field symbol. | Pops the top stack value into an extended aliased field. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopAliasedVar` | `HB_BOOL hb_xvmPopAliasedVar( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the aliased variable. | Pops the top stack value into an aliased variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopField` | `HB_BOOL hb_xvmPopField( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the field. | Pops the top stack value into a field. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopLocal` | `HB_BOOL hb_xvmPopLocal( HB_SHORT iLocal )` | `iLocal`: The local variable index. | Pops the top stack value into a local variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopLogical` | `HB_BOOL hb_xvmPopLogical( HB_BOOL * pfValue )` | `pfValue`: Pointer to store the logical value. | Pops the top stack value as a logical value. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopMemvar` | `HB_BOOL hb_xvmPopMemvar( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the memory variable. | Pops the top stack value into a memory variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPopVariable` | `HB_BOOL hb_xvmPopVariable( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the variable. | Pops the top stack value into a variable. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushAlias` | `HB_BOOL hb_xvmPushAlias( void )` | None | Pushes the current alias onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushAliasedField` | `HB_BOOL hb_xvmPushAliasedField( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the aliased field. | Pushes an aliased field onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushAliasedFieldExt` | `HB_BOOL hb_xvmPushAliasedFieldExt( PHB_SYMB pAlias, PHB_SYMB pField )` | `pAlias`: The alias symbol. <br> `pField`: The field symbol. | Pushes an extended aliased field onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushAliasedVar` | `HB_BOOL hb_xvmPushAliasedVar( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the aliased variable. | Pushes an aliased variable onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushBlock` | `void hb_xvmPushBlock( const HB_BYTE * pCode, PHB_SYMB pSymbols )` | `pCode`: The bytecode for the block. <br> `pSymbols`: The symbols for the block. | Pushes a block of code onto the stack. | None |
| `hb_xvmPushBlockShort` | `void hb_xvmPushBlockShort( const HB_BYTE * pCode, PHB_SYMB pSymbols )` | `pCode`: The bytecode for the block. <br> `pSymbols`: The symbols for the block. | Pushes a short block of code onto the stack. | None |
| `hb_xvmPushField` | `HB_BOOL hb_xvmPushField( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the field. | Pushes a field onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushFuncSymbol` | `void hb_xvmPushFuncSymbol( PHB_SYMB pSym )` | `pSym`: The function symbol. | Pushes a function symbol onto the stack. | None |
| `hb_xvmPushLocal` | `void hb_xvmPushLocal( HB_SHORT iLocal )` | `iLocal`: The local variable index. | Pushes a local variable onto the stack. | None |
| `hb_xvmPushLocalByRef` | `void hb_xvmPushLocalByRef( HB_SHORT iLocal )` | `iLocal`: The local variable index. | Pushes a local variable by reference onto the stack. | None |
| `hb_xvmPushLongLong` | `void hb_xvmPushLongLong( HB_LONGLONG llNumber )` | `llNumber`: The long long integer value. | Pushes a long long integer onto the stack. | None |
| `hb_xvmPushMemvar` | `HB_BOOL hb_xvmPushMemvar( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the memory variable. | Pushes a memory variable onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushMemvarByRef` | `HB_BOOL hb_xvmPushMemvarByRef( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the memory variable. | Pushes a memory variable by reference onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushObjectVarRef` | `HB_BOOL hb_xvmPushObjectVarRef( void )` | None | Pushes a reference to an object variable onto the stack. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmPushSelf` | `void hb_xvmPushSelf( void )` | None | Pushes the self object onto the stack. | None |
| `hb_xvmPushStatic` | `void hb_xvmPushStatic( HB_USHORT uiStatic )` | `uiStatic`: The static variable index. | Pushes a static variable onto the stack. | None |
| `hb_xvmPushStaticByRef` | `void hb_xvmPushStaticByRef( HB_USHORT uiStatic )` | `uiStatic`: The static variable index. | Pushes a static variable by reference onto the stack. | None |
| `hb_xvmPushStringHidden` | `void hb_xvmPushStringHidden( int iMethod, const char * szText, HB_SIZE nSize )` | `iMethod`: The method identifier. <br> `szText`: The string text. <br> `nSize`: The size of the string. | Pushes a hidden string onto the stack. | None |
| `hb_xvmRetInt` | `void hb_xvmRetInt( HB_LONG lValue )` | `lValue`: The integer value to return. | Returns an integer value. | None |
| `hb_xvmRetNil` | `void hb_xvmRetNil( void )` | None | Returns a nil value. | None |
| `hb_xvmRetValue` | `void hb_xvmRetValue( void )` | None | Returns the top stack value. | None |
| `hb_xvmSFrame` | `void hb_xvmSFrame( PHB_SYMB pSymbol )` | `pSymbol`: The symbol of the statics frame. | Sets the statics frame for a function. | None |
| `hb_xvmSend` | `HB_BOOL hb_xvmSend( HB_USHORT uiParams )` | `uiParams`: The number of parameters. | Sends a message with the specified number of parameters. | Returns `HB_TRUE` on success, `HB_FALSE` on failure. |
| `hb_xvmSetLine` | `void hb_xvmSetLine( HB_USHORT uiLine )` | `uiLine`: The line number. | Sets the current line number in the virtual machine. | None |
| `hb_xvmStatics` | `void hb_xvmStatics( PHB_SYMB pSymbol, HB_USHORT uiStatics )` | `pSymbol`: The symbol of the statics. <br> `uiStatics`: The number of statics. | Initializes or redimensions the global statics array. | None |
| `hb_xvmThreadStatics` | `void hb_xvmThreadStatics( HB_USHORT uiStatics, const HB_BYTE * statics )` | `uiStatics`: The number of thread statics. <br> `statics`: The statics bytecode. | Initializes thread static variables. | None |
| `hb_xvmVFrame` | `void hb_xvmVFrame( int iLocals, int iParams )` | `iLocals`: The number of local variables. <br> `iParams`: The number of parameters. | Increases the stack pointer for the specified number of locals and variable number of params. | None |

