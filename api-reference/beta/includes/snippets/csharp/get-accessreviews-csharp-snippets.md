---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fa296eb1aeec93b53408533ded13b9624cff70c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviews = await graphClient.AccessReviews
    .Request()
    .Filter("businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'")
    .Skip(0)
    .Top(100)
    .GetAsync();

```