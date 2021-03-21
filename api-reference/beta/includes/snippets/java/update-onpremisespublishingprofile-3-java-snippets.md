---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e115d7cfc2269bf2d4dfe2f1aff8360ad19f1de
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963265"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HybridAgentUpdaterConfiguration hybridAgentUpdaterConfiguration = new HybridAgentUpdaterConfiguration();
hybridAgentUpdaterConfiguration.allowUpdateConfigurationOverride = false;

graphClient.customRequest("/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration", HybridAgentUpdaterConfiguration.class)
    .buildRequest()
    .patch(hybridAgentUpdaterConfiguration);

```