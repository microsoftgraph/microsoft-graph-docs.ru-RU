---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79e6f93c1ee989ecca5348d6d284d1807f8e40a7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294607"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).Get(nil)


```