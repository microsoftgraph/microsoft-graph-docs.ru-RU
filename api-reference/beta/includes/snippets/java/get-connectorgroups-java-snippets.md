---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af195a7d64e798758770867d3e1449f157957bddcd3522db705075e7c217cbb5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57055044"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroupCollectionPage connectorGroups = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups()
    .buildRequest()
    .get();

```