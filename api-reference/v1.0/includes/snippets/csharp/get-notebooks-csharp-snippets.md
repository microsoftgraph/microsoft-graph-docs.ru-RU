---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 739acee415de72d95eedb38f3af3de451264b9040aeb98fa2c7d9389e26ebd4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57366787"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebooks = await graphClient.Me.Onenote.Notebooks
    .Request()
    .GetAsync();

```