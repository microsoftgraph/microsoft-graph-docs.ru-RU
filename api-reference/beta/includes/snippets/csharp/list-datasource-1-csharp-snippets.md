---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b52e90f25761e9152e3eca6de6ecf10d794dc4be860df576ee3025e69e9020f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var additionalSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].AdditionalSources
    .Request()
    .GetAsync();

```