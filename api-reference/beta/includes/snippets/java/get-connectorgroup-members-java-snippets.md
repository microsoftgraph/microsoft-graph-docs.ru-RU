---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fb92f128c0450ff601149009af68e9f8b73206ae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981742"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorCollectionPage members = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").members()
    .buildRequest()
    .get();

```