---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 662d66e0a5d54093c983176815df9fa364490f88
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178948"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserFlowLanguagePageCollectionPage defaultPages = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").defaultPages()
    .buildRequest()
    .get();

```