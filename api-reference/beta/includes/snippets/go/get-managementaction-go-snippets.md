---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 160a6b5d848b3694e384d4c9b4bb79480d1c8f1f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managementActionId := "managementAction-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionsById(&managementActionId).Get(options)


```