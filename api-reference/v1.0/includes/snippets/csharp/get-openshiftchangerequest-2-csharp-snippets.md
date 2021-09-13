---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 080c27b0d3cb6a57eca9103f88f52d15a09c27f042cd7126deda223d5c74f00f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57432382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShiftChangeRequests = await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests
    .Request()
    .GetAsync();

```