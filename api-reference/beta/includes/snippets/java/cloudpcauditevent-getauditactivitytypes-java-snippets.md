---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a67b1aebaf5e83f324b888fe810059c8aa7fcf2c4166c00011bba10de503f200
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57195594"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcAuditEventGetAuditActivityTypesCollectionPage getAuditActivityTypes = graphClient.deviceManagement().virtualEndpoint().auditEvents()
    .getAuditActivityTypes()
    .buildRequest()
    .get();

```