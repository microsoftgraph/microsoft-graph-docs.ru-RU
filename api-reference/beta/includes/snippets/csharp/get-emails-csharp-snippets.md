---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f2468f54d948f07e164c934daff030ba5018a199
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emails = await graphClient.Me.Profile.Emails
    .Request()
    .GetAsync();

```