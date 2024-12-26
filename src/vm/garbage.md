### Alphabetically Ordered Table of C Functions in `src/vm/garbage.c`

| Function Name          | Parameters                                              | Return Value | Description |
|------------------------|---------------------------------------------------------|--------------|-------------|
| `hb_gcAllocate`        | `HB_SIZE nSize, const HB_GC_FUNCS* pFuncs`              | `void*`      | Allocates a memory block with the specified size and functions. |
| `hb_gcAllocRaw`        | `HB_SIZE nSize, const HB_GC_FUNCS* pFuncs`              | `void*`      | Allocates a raw memory block with the specified size and functions. |
| `hb_gcAttach`          | `void* pBlock`                                          | `void`       | Attaches a memory block so it will not be released. |
| `hb_gcCollect`         | None                                                    | `void`       | Performs a garbage collection process. |
| `hb_gcCollectAll`      | `HB_BOOL fForce`                                        | `void`       | Performs a complete garbage collection process, optionally forcing it. |
| `hb_gcFree`            | `void* pBlock`                                          | `void`       | Frees a memory block allocated with `hb_gcAlloc*()` functions. |
| `hb_gcFuncs`           | `void* pBlock`                                          | `const HB_GC_FUNCS*` | Returns the cleanup function pointer for a memory block. |
| `hb_gcGripDrop`        | `PHB_ITEM pItem`                                        | `void`       | Drops a grip on a memory item. |
| `hb_gcGripGet`         | `PHB_ITEM pOrigin`                                      | `PHB_ITEM`   | Gets a grip on a memory item. |
| `hb_gcItemRef`         | `PHB_ITEM pItem`                                        | `void`       | Marks a passed item as used so it will not be released by the GC. |
| `hb_gcLock`            | `void* pBlock`                                          | `void*`      | Locks a memory block so it will not be released. |
| `hb_gcMark`            | `void* pBlock`                                          | `void`       | Marks a memory block as used so it will not be released by the GC. |
| `hb_gcRefCount`        | `void* pBlock`                                          | `HB_COUNTER` | Returns the number of references to a memory block. |
| `hb_gcRefFree`         | `void* pBlock`                                          | `void`       | Decrements the reference counter and frees the block when it reaches 0. |
| `hb_gcRefInc`          | `void* pBlock`                                          | `void`       | Increments the reference counter of a memory block. |
| `hb_gcReleaseAll`      | None                                                    | `void`       | Releases all memory blocks at the end of HVM cleanup code. |
| `hb_gcUnlock`          | `void* pBlock`                                          | `void*`      | Unlocks a memory block so it can be released if there are no references. |
| `HB_FUNC( HB_GCALL )`  | None                                                    | `void`       | Checks all memory blocks to see if they can be released. |
| `HB_FUNC( HB_GCSETAUTO )` | None                                                 | `void`       | Sets the automatic garbage collection parameters. |
| `HB_FUNC( HB_GCSTEP )` | None                                                    | `void`       | Services a single garbage collector step. |
