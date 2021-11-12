---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 53c4f7e51abea6ad14ce14b358c29e7019471e17a042b6ec3cbdc72728e5e055
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152678"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = new Room
{
    Nickname = "Conf Room",
    Building = "1",
    Label = "100",
    Capacity = 50,
    IsWheelChairAccessible = false
};

await graphClient.Places["{place-id}"]
    .Request()
    .UpdateAsync(place);

```