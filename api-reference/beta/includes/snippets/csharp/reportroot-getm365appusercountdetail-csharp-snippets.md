---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 84176d2e3b561400b0cf233ca9ee7ecb3da06bea
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Reports
    .GetM365AppUserDetail("D7").Content
    .Request()
    .GetAsync();

```