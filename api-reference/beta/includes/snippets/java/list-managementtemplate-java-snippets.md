---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 94063ce92003b0af95d8e914e90d579e03476a15c692573d257cf724b984b295
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364738"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementTemplateCollectionPage managementTemplates = graphClient.tenantRelationships().managedTenants().managementTemplates()
    .buildRequest()
    .get();

```