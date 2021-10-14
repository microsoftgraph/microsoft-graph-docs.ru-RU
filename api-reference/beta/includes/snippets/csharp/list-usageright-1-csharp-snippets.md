---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 11dd145a8410c0d7c3cff2bb267f473e7de39bb39e030eef0122201c511e80c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57055037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Devices["{device-id}"].UsageRights
    .Request()
    .GetAsync();

```