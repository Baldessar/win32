---
title: RegisteredTask.GetInstances method
description: For scripting, returns all currently running instances of the registered task.
ms.assetid: 4634851e-e868-4915-a7da-32a39f405974
keywords:
- GetInstances method Task Scheduler
- GetInstances method Task Scheduler , RegisteredTask object
- RegisteredTask object Task Scheduler , GetInstances method
topic_type:
- apiref
api_name:
- RegisteredTask.GetInstances
api_location:
- taskschd.dll
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# RegisteredTask.GetInstances method

For scripting, returns all currently running instances of the registered task.

> [!Note]  
> **RegisteredTask.GetInstances** will only return instances of the currently running registered task that are running at or below a user's security context. For example, for members of the Administrators group, **GetInstances** will return all instances of the currently running registered task, but for members of the Users group, **GetInstances** will only return instances of the currently running registered task that are running under the Users group security context.

 

## Syntax


```VB
RegisteredTask.GetInstances( _
  ByVal flags, _
  ByRef runningTasks _
)
```



## Parameters

<dl> <dt>

*flags* 
</dt> <dd>

This parameter is reserved for future use and must be set to 0.

</dd> <dt>

*runningTasks* \[out\]
</dt> <dd>

A [**RunningTaskCollection**](runningtaskcollection.md) object that contains all currently running instances of the task.

</dd> </dl>

## Return value

This method does not return a value.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                    |
| Type library<br/>             | <dl> <dt>Taskschd.tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## See also

<dl> <dt>

[Task Scheduler](task-scheduler-start-page.md)
</dt> <dt>

[**RegisteredTask**](registeredtask.md)
</dt> </dl>

 

 




