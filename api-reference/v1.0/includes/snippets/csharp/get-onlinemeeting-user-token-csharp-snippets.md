---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a12bc03a70b5aa4ae42ddd74a861c38ca6e95314d46b595932f8d8b2b479005e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"]
    .Request()
    .GetAsync();

```