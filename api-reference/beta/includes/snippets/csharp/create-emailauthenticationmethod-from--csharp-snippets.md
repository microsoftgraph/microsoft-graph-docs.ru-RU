---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e64969734186bcab996b5895c2561f4e5ba7b415a438e8cce24aa86dba1924bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = new EmailAuthenticationMethod
{
    EmailAddress = "kim@contoso.com"
};

await graphClient.Users["{user-id}"].Authentication.EmailMethods
    .Request()
    .AddAsync(emailAuthenticationMethod);

```