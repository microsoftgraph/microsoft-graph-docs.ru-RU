---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f1e19042fe6d8a2eaa8659bf04f5f88cd62be70
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comments = await graphClient.Drive.Root.Workbook.Comments
    .Request()
    .GetAsync();

```