---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d0cf8867db74cfe98d2488924e39ab0993930f533c20cdbfe0ec176e4c5a824c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["{group-id}"]
    .Request()
    .Select("allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount")
    .GetAsync();

```