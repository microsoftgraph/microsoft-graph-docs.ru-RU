---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 27e1663576b7acc3c9376dfbf7db689513e78d0a
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var invitation = new Invitation
{
    InvitedUserEmailAddress = "yyy@test.com",
    InviteRedirectUrl = "https://myapp.contoso.com"
};

await graphClient.Invitations
    .Request()
    .AddAsync(invitation);

```