---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46fb8ab7c372499d6d47d84d6f43585692900ab0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var documentSetVersions = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].DocumentSetVersions
    .Request()
    .GetAsync();

```