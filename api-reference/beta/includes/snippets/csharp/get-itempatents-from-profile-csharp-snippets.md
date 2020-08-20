---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b87dfbbb3421c452240a36b89ebe3d187e84a4f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820152"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var patents = await graphClient.Me.Profile.Patents
    .Request()
    .GetAsync();

```