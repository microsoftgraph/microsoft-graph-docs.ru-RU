---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cdf43986be210cb14fae4e6e998d9f99d243208069e71362e8b75c06e400c0d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57246676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("appDefinitions/any(a:a/allowedInstallationScopes has 'personal')")
    .Expand("appDefinitions($select=id,displayName,allowedInstallationScopes)")
    .GetAsync();

```