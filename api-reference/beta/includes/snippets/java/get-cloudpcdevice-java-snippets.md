---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c0de4a5e711335d5dba573779c3212a9e5a34ec9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440186"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDevice cloudPcDevice = graphClient.tenantRelationships().managedTenants().cloudPcDevices("{cloudPcDeviceId}")
    .buildRequest()
    .get();

```