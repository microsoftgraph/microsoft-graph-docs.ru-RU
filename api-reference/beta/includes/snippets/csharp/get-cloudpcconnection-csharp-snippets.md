---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cda4de6f5d89a52828de23f4cc4a44c694d2743c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440224"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcConnection = await graphClient.TenantRelationships.ManagedTenants.CloudPcConnections["{managedTenants.cloudPcConnection-id}"]
    .Request()
    .GetAsync();

```