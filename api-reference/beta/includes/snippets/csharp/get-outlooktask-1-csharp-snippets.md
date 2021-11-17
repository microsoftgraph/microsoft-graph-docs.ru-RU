---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1a0b7f8d3e7cb11816df8f3ec791f282c913521993807c6ecf07b67d2a97c8ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Request()
    .GetAsync();

```