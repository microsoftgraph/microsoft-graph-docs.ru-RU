---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0fae2c9a1877328203a02c2dd16c9648a6c20d0a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295645"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcDeviceId := "cloudPcDevice-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcDevicesById(&cloudPcDeviceId).Get(nil)


```