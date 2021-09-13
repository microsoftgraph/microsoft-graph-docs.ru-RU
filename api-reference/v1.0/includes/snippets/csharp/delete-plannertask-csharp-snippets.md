---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2bb19d75993ada5de5b7979bec6878514fde21d31ef212d26702e53ea419a948
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57317460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Tasks["{plannerTask-id}"]
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .DeleteAsync();

```