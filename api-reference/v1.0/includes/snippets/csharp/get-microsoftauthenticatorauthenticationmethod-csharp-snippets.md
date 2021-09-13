---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 45cd3082ed625536bdcd9d4a2a861e9531037fbb449383966d3a7921735f26fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57430687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftAuthenticatorAuthenticationMethod = await graphClient.Users["{user-id}"].Authentication.MicrosoftAuthenticatorMethods["{microsoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```