---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3e15c665d1efa156b3ef0f472dfd6931a6bf848e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871640"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerDeviceUsageUserDetailCollectionPage getYammerDeviceUsageUserDetail = graphClient.reports()
    .getYammerDeviceUsageUserDetail('D7')
    .buildRequest()
    .get();

```