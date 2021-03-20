---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3ac5b8fa08eb1f69e41aa2c2e9e9a08b7843b068
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var localizations = await graphClient.Organization["{organization-id}"].Branding.Localizations
    .Request()
    .GetAsync();

```