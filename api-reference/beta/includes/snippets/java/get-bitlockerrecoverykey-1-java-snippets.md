---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2514c7c54a77913d5298f47b29d9cde31234e58b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210513"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ocp-client-name", "\"My Friendly Client\""));
requestOptions.add(new HeaderOption("ocp-client-version", "\"1.2\""));

BitlockerRecoveryKeyCollectionPage recoveryKeys = graphClient.informationProtection().bitlocker().recoveryKeys()
    .buildRequest( requestOptions )
    .get();

```