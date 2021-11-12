---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e7b2c41b569dc6c57ef0ecbe35739ae44250fe25ce74df14d9afd8ec93bf14f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .GetAsync();

```