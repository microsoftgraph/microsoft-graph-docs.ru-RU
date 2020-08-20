---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07c1c596a3aa82032b56e8d3c2013f4f218699fd
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var awards = await graphClient.Me.Profile.Awards
    .Request()
    .GetAsync();

```