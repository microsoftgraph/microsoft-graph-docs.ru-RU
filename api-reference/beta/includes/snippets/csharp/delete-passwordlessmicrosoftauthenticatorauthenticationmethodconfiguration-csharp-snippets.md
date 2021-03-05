---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7facc676d9fd528e32d413acd532af77c28def47
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["passwordlessMicrosoftAuthenticator"]
    .Request()
    .DeleteAsync();

```