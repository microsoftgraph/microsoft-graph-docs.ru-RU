---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e87af6405da76d836d26ec512780e7f723602a386299df5934b6a1dde448dd56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57209534"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegration = await graphClient.Teamwork.WorkforceIntegrations["{workforceIntegration-id}"]
    .Request()
    .GetAsync();

```