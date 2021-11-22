---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f0473dc59446fae38bc15ccb66eadbe32c25e711a24a8c7684026aed9ec5127
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57270210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordAuthenticationMethod = await graphClient.Me.Authentication.PasswordMethods["{passwordAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```