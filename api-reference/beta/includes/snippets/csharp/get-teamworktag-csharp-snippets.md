---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6a4bf7eeb56d544e1ec6d2b74ce3475eebe947a7eafbbf02df5c6419b748ea8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57251779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkTag = await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"]
    .Request()
    .GetAsync();

```