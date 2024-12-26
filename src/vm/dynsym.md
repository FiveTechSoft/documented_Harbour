Alphabetically Ordered Table of C Functions in src/vm/dynsym.c
hb_dynsymAreaHandle	PHB_DYNS pDynSym	int: Area handle
hb_dynsymByItem	PHB_ITEM pItem	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymCount	None	HB_LONG: Number of dynamic symbols
hb_dynsymEval	PHB_DYNS_FUNC pFunction, void * Cargo	void
hb_dynsymFind	const char * szName	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymFindName	const char * szName	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymFindSymbol	const char * szName	PHB_SYMB: Pointer to symbol
hb_dynsymFromNum	HB_SYMCNT uiSymNum	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymGet	const char * szName	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymGetByIndex	HB_LONG lIndex	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymGetCase	const char * szName	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymGetMemvar	PHB_DYNS pDynSym	PHB_ITEM: Memory variable
hb_dynsymGetSymbol	const char * szName	PHB_SYMB: Pointer to symbol
hb_dynsymInsert	PHB_SYMB pSymbol, HB_SYMCNT uiPos	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymIsFunction	PHB_DYNS pDynSym	HB_BOOL: TRUE if it is a function
hb_dynsymIsMemvar	PHB_DYNS pDynSym	HB_BOOL: TRUE if it is a memory variable
hb_dynsymName	PHB_DYNS pDynSym	const char *: Name of the dynamic symbol
hb_dynsymNew	PHB_SYMB pSymbol	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymPos	const char * szName, HB_SYMCNT * puiPos	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymProtectEval	PHB_DYNS_FUNC pFunction, void * Cargo	void
hb_dynsymRelease	None	void
hb_dynsymSetAreaHandle	PHB_DYNS pDynSym, int iArea	void
hb_dynsymSetMemvar	PHB_DYNS pDynSym, PHB_ITEM pMemvar	void
hb_dynsymSymbol	PHB_DYNS pDynSym	PHB_SYMB: Pointer to symbol
hb_dynsymToNum	PHB_DYNS pDynSym	HB_SYMCNT: Symbol number
hb_dynsymVerify	None	int: Result of verification
hb_symbolAlloc	const char * szName	PHB_SYMB: Pointer to symbol
hb_symbolNew	const char * szName	PHB_SYMB: Pointer to symbol
hb_dynsymInsert	PHB_SYMB pSymbol, HB_SYMCNT uiPos	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymPos	const char * szName, HB_SYMCNT * puiPos	PHB_DYNS: Pointer to dynamic symbol
hb_dynsymProtectEval	PHB_DYNS_FUNC pFunction, void * Cargo	void
hb_dynsymRelease	None	void
hb_dynsymSetAreaHandle	PHB_DYNS pDynSym, int iArea	void
hb_dynsymSetMemvar	PHB_DYNS pDynSym, PHB_ITEM pMemvar	void
hb_dynsymSymbol	PHB_DYNS pDynSym	PHB_SYMB: Pointer to symbol
hb_dynsymToNum	PHB_DYNS pDynSym	HB_SYMCNT: Symbol number
hb_dynsymVerify	None	int: Result of verification
hb_symbolAlloc	const char * szName	PHB_SYMB: Pointer to symbol
hb_symbolNew	const char * szName	PHB_SYMB: Pointer to symbol
