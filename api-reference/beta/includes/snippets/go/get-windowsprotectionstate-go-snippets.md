---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3197a73814e0f4de90706043af8c943b1bd75547
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011829"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

windowsProtectionStateId := "windowsProtectionState-id"
result, err := graphClient.TenantRelationships().ManagedTenants().WindowsProtectionStatesById(&windowsProtectionStateId).Get(options)


```