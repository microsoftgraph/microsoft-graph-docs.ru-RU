---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 010676d832e6dc6e1d27106974113c0a0e44870e39d57792cacbcfddaf73b90b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57313910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"]
    .Request()
    .GetAsync();

```