---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4b0ebb7261e85c36ecd00e31baa8c14c35d83e62425bbbbb072fa7de96618c50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57193419"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Tenant tenant = graphClient.tenantRelationships().managedTenants().tenants("{tenantId}")
    .buildRequest()
    .get();

```