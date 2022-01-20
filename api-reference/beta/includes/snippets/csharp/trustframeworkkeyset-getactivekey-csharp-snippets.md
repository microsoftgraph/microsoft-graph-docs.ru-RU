---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c4a27ab757c8878d97c85b091145a02af49c59093389af14a4e56ae2a5d848aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57310108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trustFrameworkKey = await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .GetActiveKey()
    .Request()
    .GetAsync();

```