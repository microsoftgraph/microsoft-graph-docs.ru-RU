---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b3e6223803d987bc1a2305f18e67836ffd468674
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrgContactDeltaCollectionPage delta = graphClient.contacts()
    .delta()
    .buildRequest()
    .select("displayName,jobTitle,mail")
    .get();

```