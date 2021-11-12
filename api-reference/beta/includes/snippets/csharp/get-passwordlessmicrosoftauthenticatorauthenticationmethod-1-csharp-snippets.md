---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eafe04a660a35483a010e6f89043fbab3b632718d142749334da983dcd44f4da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordlessMicrosoftAuthenticatorAuthenticationMethod = await graphClient.Me.Authentication.PasswordlessMicrosoftAuthenticatorMethods["{passwordlessMicrosoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```