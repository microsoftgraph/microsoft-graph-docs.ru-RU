---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2493f7b49559e44bd0739212bb6c80d3bf1a4588bf695783cfc5072313ff28d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57246696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("id eq '876df28f-2e78-423b-94a5-44181bd0e225'")
    .Expand("appDefinitions")
    .GetAsync();

```