---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14a0af37432eb4d8b66ba0dc690a04f10159a0dc9721f6a6c3bd8613b2c15532
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57313256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request()
    .GetAsync();

```