---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bfe6ee03c0a4336f2f52708cd572ea2384caa4a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordlessMicrosoftAuthenticatorMethods = await graphClient.Me.Authentication.PasswordlessMicrosoftAuthenticatorMethods
    .Request()
    .GetAsync();

```