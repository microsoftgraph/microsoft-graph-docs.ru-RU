---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 39ae3b7873a5f79e4c3eb58e101f665c295ab0c55231179c29f2a5454c0552b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57248403"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "String";

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Abort(reason)
    .Request()
    .PostAsync();

```