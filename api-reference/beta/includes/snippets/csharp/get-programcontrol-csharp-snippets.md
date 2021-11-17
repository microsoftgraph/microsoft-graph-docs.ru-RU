---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68a39fbc0e3717472a662c96c2f4e8cd1c30888e31d608558886ded017e6cf0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57323688"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControls = await graphClient.ProgramControls
    .Request()
    .GetAsync();

```