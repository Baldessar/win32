---
Description: Gets a custom device icon.
ms.assetid: 27763f39-80d8-4862-b045-e49c6e824c28
title: IWiaUIExtension::GetDeviceIcon method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IWiaUIExtension::GetDeviceIcon method

Gets a custom device icon.

## Syntax


```C++
HRESULT GetDeviceIcon(
  [in]  BSTR  bstrDeviceId,
  [out] HICON *phIcon,
  [in]  ULONG nSize
);
```



## Parameters

<dl> <dt>

*bstrDeviceId* \[in\]
</dt> <dd>

Type: **BSTR**

Specifies the device ID of the WIA device for which the icon is to be obtained.

</dd> <dt>

*phIcon* \[out\]
</dt> <dd>

Type: **HICON\***

Points to a memory location that will receive a handle for the icon for the device.

</dd> <dt>

*nSize* \[in\]
</dt> <dd>

Type: **ULONG**

Specifies the desired icon size, in pixels. The icon is assumed to be square, and nSize specifies both the width and height of the requested icon.

</dd> </dl>

## Return value

Type: **HRESULT**

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements



|                                     |                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                 |
| Header<br/>                   | <dl> <dt>Wiadevd.h</dt> </dl> |



 

 



