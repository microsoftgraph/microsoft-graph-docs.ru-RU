---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ac85c451c1006c9b6c786615da6c05b0804fe2c1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978310"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationId := "application-id"
federatedIdentityCredentialId := "federatedIdentityCredential-id"
result, err := graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Get(options)


```