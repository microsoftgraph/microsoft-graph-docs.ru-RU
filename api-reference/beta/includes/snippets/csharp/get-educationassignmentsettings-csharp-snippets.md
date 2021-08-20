---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b6a91279e50b2c3d73c08e114fcc8eb65ae2b03ce62f10b156376b85d51de31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57365476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentSettings = await graphClient.Education.Classes["{educationClass-id}"].AssignmentSettings
    .Request()
    .GetAsync();

```