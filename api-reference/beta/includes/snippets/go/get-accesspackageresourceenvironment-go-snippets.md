---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 73b3c74b969abf861238f090e78ae6b2f75f1fb8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294554"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageResourceEnvironmentId := "accessPackageResourceEnvironment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceEnvironmentsById(&accessPackageResourceEnvironmentId).Get(nil)


```