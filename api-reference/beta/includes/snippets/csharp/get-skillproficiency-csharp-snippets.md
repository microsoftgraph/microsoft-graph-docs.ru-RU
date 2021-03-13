---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c22f3e6326c9412c489de27210406248b2e24112
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = await graphClient.Me.Profile.Skills["{skillProficiency-id}"]
    .Request()
    .GetAsync();

```