---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a2bae6948726bd19a3c74ff5fd8b9619b6d0156eb1e8e3c3a209bcd4094866f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57368538"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOnPremisesConnectionCollectionPage onPremisesConnections = graphClient.deviceManagement().virtualEndpoint().onPremisesConnections()
    .buildRequest()
    .get();

```