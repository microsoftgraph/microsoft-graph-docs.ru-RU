---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca8f9d87ce0baa79b2201c283a2080a881a3dd9c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445436"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskGroups = await graphClient.Me.Outlook.TaskGroups
    .Request()
    .GetAsync();

```