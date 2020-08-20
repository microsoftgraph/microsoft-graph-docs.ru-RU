---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 927bb49b4410d2156ae45d4729caef297e363a32
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819406"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notes = await graphClient.Me.Profile.Notes
    .Request()
    .GetAsync();

```