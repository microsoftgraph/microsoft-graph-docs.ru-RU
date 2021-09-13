---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 84f4c1ea4dcc4ff3f0c7aea86f118c428f4528198f495820735e38506f1fc813
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203418"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders["{mailFolder-id}"].Messages
    .Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .GetAsync();

```