---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5c18fbf04cc56e5dd879d39fabedbe3fccd65bae
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212679"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SimulationAutomationRunCollectionPage runs = graphClient.security().attackSimulation().simulationAutomations("fbad62b0-b32d-b6ac-9f48-d84bbea08f96").runs()
    .buildRequest()
    .get();

```