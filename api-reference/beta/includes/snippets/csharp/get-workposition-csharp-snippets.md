---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ba46d3db12cf77dbaa682ca6839e31feb929cfef6981d5469b94cf613a38fd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57204766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workPosition = await graphClient.Me.Profile.Positions["{workPosition-id}"]
    .Request()
    .GetAsync();

```