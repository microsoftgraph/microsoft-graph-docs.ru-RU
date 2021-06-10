---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9b00d5b26c4d3b56786dadaf4003b00653b3a302
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getUserArchivedPrintJobs = await graphClient.Print.Reports
    .GetUserArchivedPrintJobs("016b5565-3bbf-4067-b9ff-4d68167eb1a6","2021-05-24","2021-05-25")
    .Request()
    .GetAsync();

```