---
Description: Terminates the trace.
ms.assetid: e823ed82-1966-4e44-b062-0c8ab0fb5f6e
title: TermAsyncTrace function
ms.topic: reference
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- TermAsyncTrace
api_type: 
- DllExport
api_location: 
- Exstrace.dll
---

# TermAsyncTrace function

Terminates the trace.

## Syntax


```C++
BOOL TermAsyncTrace(void);
```



## Parameters

This function has no parameters.

## Return value

This function returns **TRUE** if it succeeds; otherwise, it returns **FALSE**.

## Remarks

Exstrace.dll is an optional component that installs with the Simple Mail Transfer Protocol (SMTP) and the Network News Transfer Protocol (NNTP).

This function has no associated import library or header file; you must call it using the [**LoadLibrary**](https://msdn.microsoft.com/library/ms684175(v=VS.85).aspx) and [**GetProcAddress**](https://msdn.microsoft.com/library/ms683212(v=VS.85).aspx) functions.

## Requirements



|                |                                                                                         |
|----------------|-----------------------------------------------------------------------------------------|
| DLL<br/> | <dl> <dt>Exstrace.dll</dt> </dl> |



 

 




