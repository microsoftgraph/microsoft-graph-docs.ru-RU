---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7f4a0f5ab6a625d9e1846023e8df36030fd4dd54bf5e014d304a7634dc9694fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57366646"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceCollectionPage cloudPcDevices = graphClient.tenantRelationships().managedTenants().cloudPcDevices()
    .buildRequest()
    .get();

```