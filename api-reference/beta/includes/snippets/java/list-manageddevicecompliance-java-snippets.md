---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2531762afe8bba8a1ba60ee538c1bbeae482b978
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442052"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceComplianceCollectionPage managedDeviceCompliances = graphClient.tenantRelationships().managedTenants().managedDeviceCompliances()
    .buildRequest()
    .get();

```