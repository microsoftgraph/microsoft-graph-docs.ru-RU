---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 768102a622568b6adb0d90305d30340209812401d67d4d37f60f3f44d04222fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138570"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = await graphClient.AccessReviews["{accessReview-id}"]
    .Request()
    .GetAsync();

```