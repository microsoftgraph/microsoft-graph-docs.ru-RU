---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ea320e4934139aa184c7176ce448e04034b6d7d96c04b0cab1563266f1c01ce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{contactFolder-id}"].Contacts
    .Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .Select("displayName")
    .GetAsync();

```