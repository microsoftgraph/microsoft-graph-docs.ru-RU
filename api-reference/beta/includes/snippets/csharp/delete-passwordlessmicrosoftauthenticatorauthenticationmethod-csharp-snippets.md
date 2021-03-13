---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c7eca10bb162b455a7da0b210a5f52b39aee2fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.PasswordlessMicrosoftAuthenticatorMethods["{passwordlessMicrosoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```