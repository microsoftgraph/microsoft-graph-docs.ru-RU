---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 69762d057c18edc282cd217fca59d9610362d806
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723777"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calculationType = "calculationType-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Application
    .Calculate(calculationType)
    .Request()
    .PostAsync();

```