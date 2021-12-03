---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8a1471a688ebed4dce6fa2fed2ab403912c5aa42
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295166"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenIssuancePolicyId := "tokenIssuancePolicy-id"
graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Delete(nil)


```