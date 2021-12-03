---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7553d3c4732c27c8b5525bec1e736d314d45dcf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295260"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantCustomizedInformationId := "tenantCustomizedInformation-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsCustomizedInformationById(&tenantCustomizedInformationId).Get(nil)


```