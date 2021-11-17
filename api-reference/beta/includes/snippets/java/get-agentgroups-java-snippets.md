---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3bca0c006fc11b4dc6ba06c39259a43eed9380d2c45b6a87fde0490860ba5d41
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57361439"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentGroupCollectionPage agentGroups = graphClient.onPremisesPublishingProfiles("provisioning").agentGroups()
    .buildRequest()
    .expand("publishedResources")
    .get();

```