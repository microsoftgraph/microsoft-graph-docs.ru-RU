---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c237d6fac9d558c6f70072b723d7c773324f70c
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752871"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"));

graphClient.applications("{id}").connectorGroup().reference()
    .buildRequest()
    .put(connectorGroup);

```