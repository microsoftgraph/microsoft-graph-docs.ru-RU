---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 083a2c5e971ba8ea4138e28de6f385a1c48fe5d625a8cb584e4240c9e7245f09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57189314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = await graphClient.Teams["{team-id}"].Schedule.Shifts["{shift-id}"]
    .Request()
    .GetAsync();

```