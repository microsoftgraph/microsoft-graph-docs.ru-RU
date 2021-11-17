---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d52517f4095130d9b64795f9be9058d4ce991a511b87177569c0dcd045c5a8cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252189"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "deleteditems";

graphClient.me().messages("AAMkADhAAATs28OAAA=")
    .move(MessageMoveParameterSet
        .newBuilder()
        .withDestinationId(destinationId)
        .build())
    .buildRequest()
    .post();

```