---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 786b37b8c1c5f1075b436575df64ed4b0d071f9e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var methods = await graphClient.Me.Authentication.Methods
    .Request()
    .GetAsync();

```