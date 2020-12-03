---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e04ba6e555e8f1dc9b4220adf1668b8dcd94526
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522351"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IVirtualEndpointGetEffectivePermissionsCollectionPage getEffectivePermissions = graphClient.deviceManagement().virtualEndpoint()
    .getEffectivePermissions()
    .buildRequest()
    .get();

```