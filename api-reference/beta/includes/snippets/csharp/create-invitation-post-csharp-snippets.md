---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f40db6a2a81f91661c02909e5931985d6fa0657b
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var invitation = new Invitation
{
    InvitedUserEmailAddress = "admin@fabrikam.com",
    InviteRedirectUrl = "https://myapp.contoso.com"
};

await graphClient.Invitations
    .Request()
    .AddAsync(invitation);

```