---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b95dcef37921e85f611d1e821a05486a154376354e4b3c0a680ad970701e455
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394013"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationContextClassReference = new AuthenticationContextClassReference
{
    Id = "c1",
    DisplayName = "Contoso medium",
    Description = "Medium protection level defined for Contoso policy",
    IsAvailable = true
};

await graphClient.Identity.ConditionalAccess.AuthenticationContextClassReferences
    .Request()
    .AddAsync(authenticationContextClassReference);

```