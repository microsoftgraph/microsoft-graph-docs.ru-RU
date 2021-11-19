---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c005351e4a5c9ef28d5ad230a8e4798cf4d63e00
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082246"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).AccessPackagesIncompatibleWith().Get(options)


```