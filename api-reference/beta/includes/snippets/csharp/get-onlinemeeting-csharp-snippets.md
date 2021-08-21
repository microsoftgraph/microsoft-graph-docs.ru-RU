---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d6b00736a676eb40a0eec7d3b8d9456a2e032b9435ea59acd12116b27af01021
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeetings = await graphClient.Communications.OnlineMeetings
    .Request()
    .Filter("VideoTeleconferenceId eq '123456789'")
    .GetAsync();

```