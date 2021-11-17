---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0fc466493eaea6f92924875f05dee4fcb06faeec
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999915"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserFlowIdentityProviders().Get(options)


```