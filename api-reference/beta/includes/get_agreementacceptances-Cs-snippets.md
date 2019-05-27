---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f151b8dbc27407d5af305545cdec9888b79bee8a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreementAcceptances = await graphClient.Me.AgreementAcceptances
    .Request()
    .GetAsync();

```