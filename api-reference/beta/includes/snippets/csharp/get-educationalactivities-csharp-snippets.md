---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 67cd22d60567d27ef2da445429520c302e4365b84ebb3a55a6cb2dff76f7ef4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivities = await graphClient.Me.Profile.EducationalActivities
    .Request()
    .GetAsync();

```