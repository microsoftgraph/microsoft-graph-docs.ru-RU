---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5a7ae4b8f6b95020104c6b25a8b6c14dc0cf7db4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profile = await graphClient.Me.Profile
    .Request()
    .Expand("skills($select=displayName)")
    .GetAsync();

```