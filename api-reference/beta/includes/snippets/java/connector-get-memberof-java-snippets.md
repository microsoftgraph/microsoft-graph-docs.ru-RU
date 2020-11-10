---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e2c216f22a6dbddc017248b1648eb7b11a8152db
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957505"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConnectorGroupCollectionPage memberOf = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}").memberOf()
    .buildRequest()
    .get();

```