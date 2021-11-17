---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dddbdbf7229218070a34a8e43733c165fbbf8de55361c249383e0d00c80e370b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57258925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().inferenceClassification().overrides("98f5bdef-576a-404d-a2ea-07a3cf34af4r")
    .buildRequest()
    .delete();

```