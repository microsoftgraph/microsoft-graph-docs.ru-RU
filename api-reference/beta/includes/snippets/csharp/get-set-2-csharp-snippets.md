---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8971fec42b4b7c4b111942f1f91d20a2ace22d722f71ceb5e8adf0646b0beed2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57313895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = await graphClient.TermStore.Sets["{termStore.set-id}"]
    .Request()
    .GetAsync();

```