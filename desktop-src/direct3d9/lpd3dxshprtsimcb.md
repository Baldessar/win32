---
Description: Callback function for Precomputed Radiance Transfer (PRT) simulation and compression.
ms.assetid: 1d7e2149-d2ca-47da-be1f-8273fd9bd30a
title: LPD3DXSHPRTSIMCB
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# LPD3DXSHPRTSIMCB

Callback function for Precomputed Radiance Transfer (PRT) simulation and compression.

## Syntax


```
typedef HRESULT (WINAPI *LPD3DXSHPRTSIMCB)(
    FLOAT fPercentDone,
    LPVOID lpUserContext
);
```



## Parameters

fPercentDone - Floating point number between 0 and 1.0 that represents the percentage of calculations completed (between 0 and 100 percent).

lpUserContext - Pointer to a user-defined value which is passed to the callback function; typically used by an application to pass a pointer to a data structure that provides context information for the callback function.

## Return Value

This function must be implemented to return S\_OK to keep running the simulator. Any other value will halt the simulator.

## Remarks

Be sure to specify the [**Windows Data Types**](https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46) calling convention when declaring the callback function. Otherwise, stack overflows can occur.



|                          |             |
|--------------------------|-------------|
| Header                   | d3dx9mesh.h |
| Import Library           | d3dx9.lib   |
| Minimum Operating System | Windows 98  |



 

## Related topics

<dl> <dt>

[Callback Functions](dx9-graphics-reference-d3dx-callback-functions.md)
</dt> </dl>

 

 


