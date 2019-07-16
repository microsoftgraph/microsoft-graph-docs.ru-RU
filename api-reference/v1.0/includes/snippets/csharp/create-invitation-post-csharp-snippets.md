---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff3ee57a389310bc8fa1d7bd384e961710c4a4db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var invitation = new Invitation
{
    InvitedUserEmailAddress = "yyy@test.com",
    InviteRedirectUrl = "https://myapp.com"
};

await graphClient.Invitations
    .Request()
    .AddAsync(invitation);

```