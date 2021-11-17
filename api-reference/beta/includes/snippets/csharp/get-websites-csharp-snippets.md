---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c819271b97102c49848374ea9786b0a470f8ab77d61a2761566bb98647e9904
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57208655"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var websites = await graphClient.Me.Profile.Websites
    .Request()
    .GetAsync();

```