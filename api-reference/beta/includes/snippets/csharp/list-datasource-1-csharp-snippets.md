---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 052d23c4d155b98f0289e92fafbb5dec11eef48c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952149"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var additionalSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].AdditionalSources
    .Request()
    .GetAsync();

```