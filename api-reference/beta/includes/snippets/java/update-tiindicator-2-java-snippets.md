---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d4be1d97c1e89b719ecacce2d49dfd302d94ad7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942175"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.additionalInformation = "additionalInformation-after-update";
tiIndicator.confidence = 42;
tiIndicator.description = "description-after-update";

graphClient.security().tiIndicators("{id}")
    .buildRequest( requestOptions )
    .patch(tiIndicator);

```