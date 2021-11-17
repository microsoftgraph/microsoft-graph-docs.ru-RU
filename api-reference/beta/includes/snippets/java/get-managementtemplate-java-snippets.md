---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 67509c46150df277f8a07aa872bf29c206a8a4a29a468b899c069abae140ca4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57311453"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementTemplate managementTemplate = graphClient.tenantRelationships().managedTenants().managementTemplates("{managementTemplateId}")
    .buildRequest()
    .get();

```