### Alphabetically Ordered Table of C Functions in `src/vm/hashes.c`

| Function Name          | Parameters                                              | Return Value | Description |
|------------------------|---------------------------------------------------------|--------------|-------------|
| `hb_hashAdd`           | `PHB_ITEM pHash, PHB_ITEM pKey, PHB_ITEM pValue`        | `HB_BOOL`    | Adds or updates a key-value pair in the hash table. |
| `hb_hashAddNew`        | `PHB_ITEM pHash, PHB_ITEM pKey, PHB_ITEM pValue`        | `HB_BOOL`    | Adds a new key-value pair to the hash table if the key does not already exist. |
| `hb_hashAllocNewPair`  | `PHB_ITEM pHash, PHB_ITEM* pKeyPtr, PHB_ITEM* pValPtr`  | `HB_BOOL`    | Allocates space for a new key-value pair in the hash table. |
| `hb_hashClear`         | `PHB_ITEM pHash`                                        | `HB_BOOL`    | Clears all key-value pairs from the hash table. |
| `hb_hashClearFlags`    | `PHB_ITEM pHash, int iFlags`                            | `void`       | Clears specific flags from the hash table. |
| `hb_hashClone`         | `PHB_ITEM pHash`                                        | `PHB_ITEM`   | Clones the hash table into a new item. |
| `hb_hashCloneBody`     | `PHB_ITEM pDest, PHB_ITEM pHash, PHB_NESTED_CLONED pClonedList` | `void`       | Clones the body of the hash table into another item. |
| `hb_hashCloneTo`       | `PHB_ITEM pDest, PHB_ITEM pHash`                        | `PHB_ITEM`   | Clones the hash table into a specified item. |
| `hb_hashDel`           | `PHB_ITEM pHash, PHB_ITEM pKey`                         | `HB_BOOL`    | Deletes a key-value pair from the hash table by key. |
| `hb_hashDelAt`         | `PHB_ITEM pHash, HB_SIZE nPos`                          | `HB_BOOL`    | Deletes a key-value pair from the hash table by position. |
| `hb_hashDelPair`       | `PHB_BASEHASH pBaseHash, HB_SIZE nPos`                  | `void`       | Deletes a specific key-value pair from the base hash table. |
| `hb_hashFind`          | `PHB_BASEHASH pBaseHash, PHB_ITEM pKey, HB_SIZE* pnPos` | `HB_BOOL`    | Finds a key in the base hash table and returns its position. |
| `hb_hashGarbageMark`   | `void* Cargo`                                           | `void`       | Marks the garbage collector items in the hash table. |
| `hb_hashGarbageRelease`| `void* Cargo`                                           | `void`       | Releases the garbage collected items in the hash table. |
| `hb_hashGetCItemPtr`   | `PHB_ITEM pHash, const char* pszKey`                    | `PHB_ITEM`   | Gets a value from the hash table by a string key. |
| `hb_hashGetCItemPos`   | `PHB_ITEM pHash, const char* pszKey`                    | `HB_SIZE`    | Gets the position of a key in the hash table by a string key. |
| `hb_hashGetDefault`    | `PHB_ITEM pHash`                                        | `PHB_ITEM`   | Gets the default value for the hash table. |
| `hb_hashGetItemPtr`    | `PHB_ITEM pHash, PHB_ITEM pKey, int iFlags`             | `PHB_ITEM`   | Gets a value from the hash table by key with specific flags. |
| `hb_hashGetItemRefPtr` | `PHB_ITEM pHash, PHB_ITEM pKey`                         | `PHB_ITEM`   | Gets a reference to a value from the hash table by key. |
| `hb_hashGetKeyAt`      | `PHB_ITEM pHash, HB_SIZE nPos`                          | `PHB_ITEM`   | Gets a key from the hash table at a specific position. |
| `hb_hashGetKeys`       | `PHB_ITEM pHash`                                        | `PHB_ITEM`   | Gets all keys from the hash table as an array. |
| `hb_hashGetValueAt`    | `PHB_ITEM pHash, HB_SIZE nPos`                          | `PHB_ITEM`   | Gets a value from the hash table at a specific position. |
| `hb_hashGetValues`     | `PHB_ITEM pHash`                                        | `PHB_ITEM`   | Gets all values from the hash table as an array. |
| `hb_hashId`            | `PHB_ITEM pHash`                                        | `void*`      | Retrieves the unique ID of the hash table. |
| `hb_hashJoin`          | `PHB_ITEM pDest, PHB_ITEM pSource, int iType`           | `void`       | Joins two hash tables based on the specified type. |
| `hb_hashLen`           | `PHB_ITEM pHash`                                        | `HB_SIZE`    | Gets the number of key-value pairs in the hash table. |
| `hb_hashNew`           | `PHB_ITEM pItem`                                        | `PHB_ITEM`   | Creates a new hash table. |
| `hb_hashNewPair`       | `PHB_BASEHASH pBaseHash, PHB_ITEM* pKeyPtr, PHB_ITEM* pValPtr` | `void`       | Creates a new key-value pair in the base hash table. |
| `hb_hashNewValue`      | `PHB_BASEHASH pBaseHash, PHB_ITEM pKey, PHB_ITEM pValue` | `HB_BOOL`    | Adds a new key-value pair to the base hash table if the key does not already exist. |
| `hb_hashPreallocate`   | `PHB_ITEM pHash, HB_SIZE nNewSize`                      | `void`       | Preallocates space for a specified number of key-value pairs in the hash table. |
| `hb_hashRefs`          | `PHB_ITEM pHash`                                        | `HB_COUNTER` | Gets the number of references to the hash table. |
| `hb_hashRemove`        | `PHB_ITEM pHash, PHB_ITEM pItem`                        | `HB_BOOL`    | Removes key-value pairs from the hash table based on the specified item. |
| `hb_hashResize`        | `PHB_BASEHASH pBaseHash, HB_SIZE nNewSize`              | `void`       | Resizes the base hash table. |
| `hb_hashScan`          | `PHB_ITEM pHash, PHB_ITEM pKey, HB_SIZE* pnPos`         | `HB_BOOL`    | Scans the hash table for a key and returns its position. |
| `hb_hashScanSoft`      | `PHB_ITEM pHash, PHB_ITEM pKey, HB_SIZE* pnPos`         | `HB_BOOL`    | Scans the hash table for a key and returns its position, handling soft matches. |
| `hb_hashSetDefault`    | `PHB_ITEM pHash, PHB_ITEM pValue`                       | `void`       | Sets the default value for the hash table. |
| `hb_hashSetFlags`      | `PHB_ITEM pHash, int iFlags`                            | `void`       | Sets specific flags for the hash table. |
| `hb_hashSort`          | `PHB_ITEM pHash`                                        | `void`       | Sorts the hash table. |
| `hb_hashSortDo`        | `PHB_BASEHASH pBaseHash`                                | `void`       | Performs the sorting operation on the base hash table. |
| `hb_hashValuePtr`      | `PHB_BASEHASH pBaseHash, PHB_ITEM pKey, HB_BOOL fAdd`   | `PHB_ITEM`   | Gets a pointer to a value in the base hash table by key, optionally adding the key if it does not exist. |
