---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b7d22001f8118d5b934a1b256225a829d3760ebe
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenLifetimePolicyId := "tokenLifetimePolicy-id"
result, err := graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Get(options)


```