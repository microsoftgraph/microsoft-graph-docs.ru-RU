---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ec0ce181092b72bc17ea5eb72dd4fe2c9e948812ad5f37a21c02e0bffa5204c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57054946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Print.Services["{printService-id}"].Endpoints
    .Request()
    .GetAsync();

```