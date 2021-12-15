---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fb1992c70142f7ef5e231c3bc2566b8f22a0e432
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525894"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String targetServicePlanId = "30d0e128-de93-41dc-89ec-33d84bb662a0";

graphClient.deviceManagement().managedDevices("{managedDeviceId}")
    .resizeCloudPc(ManagedDeviceResizeCloudPcParameterSet
        .newBuilder()
        .withTargetServicePlanId(targetServicePlanId)
        .build())
    .buildRequest()
    .post();

```