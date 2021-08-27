---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d97723635a822aaa839e4059dca8afb7e727d7f716e05144ee0136050a85aa5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57321828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .Request()
    .DeleteAsync();

```