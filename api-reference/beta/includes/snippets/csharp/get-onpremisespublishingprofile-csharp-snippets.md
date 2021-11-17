---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 36e66ca35d276c56aec7cc985fd8acfd8ac6dfbc0ad8ef0cd1d9c25ce16cede6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesPublishingProfile = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```