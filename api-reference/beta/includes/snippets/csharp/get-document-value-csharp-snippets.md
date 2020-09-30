---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0671a651e4d503d563998bafa376b40c93a4c099
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Print.Printers["fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a"].Jobs["46140"].Documents["bd260b1a-044e-4ca6-afa9-17d9a587d254"].Content
    .Request()
    .GetAsync();

```