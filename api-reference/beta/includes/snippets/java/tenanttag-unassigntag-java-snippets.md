---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 08d5e4c774d06d3c78e2228a26a952310146eed0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442783"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> tenantIdsList = new LinkedList<String>();
tenantIdsList.add("String");

graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .unassignTag(TenantTagUnassignTagParameterSet
        .newBuilder()
        .withTenantIds(tenantIdsList)
        .build())
    .buildRequest()
    .post();

```