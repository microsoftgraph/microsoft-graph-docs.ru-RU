---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d65a9da2d8a0501f3e871b92887711fa586a9793bdb842d3fd0cb534677eddb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144604"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columnDefinition = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"].Columns["{columnDefinition-id}"]
    .Request()
    .GetAsync();

```