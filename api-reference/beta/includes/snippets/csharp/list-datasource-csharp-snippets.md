---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 47c2826cabfff5ddcf9baec95b11b1104661e4d9bf2602a954c8a490c037d1f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources["{ediscovery.noncustodialDataSource-id}"].DataSource
    .Request()
    .GetAsync();

```