---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba99913f0232729d3b67a403324ac5cf00ad83685044658fa9f99892588f86db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57267208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceConfigurationRecords = await graphClient.Domains["{domain-id}"].ServiceConfigurationRecords
    .Request()
    .GetAsync();

```