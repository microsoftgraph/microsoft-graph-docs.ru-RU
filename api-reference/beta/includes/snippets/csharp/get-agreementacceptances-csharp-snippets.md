---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f151b8dbc27407d5af305545cdec9888b79bee8a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528479"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreementAcceptances = await graphClient.Me.AgreementAcceptances
    .Request()
    .GetAsync();

```