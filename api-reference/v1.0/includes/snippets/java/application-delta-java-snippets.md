---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64e917e0531c115ac281cd4f320c0d1be776246e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806658"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IApplicationDeltaCollectionPage delta = graphClient.applications()
    .delta()
    .buildRequest()
    .get();

```