---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f2fd1ce3fd44bf3b9f31565028b96997ae13c42
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030051"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcConnectionId := "cloudPcConnection-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcConnectionsById(&cloudPcConnectionId).Get(options)


```