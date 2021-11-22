---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18e429561c637adda15a7d0ec54ecd4adc4bcb7ab964223fb1501ff78d3dfe6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203922"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicatorCollectionPage tiIndicators = graphClient.security().tiIndicators()
    .buildRequest()
    .get();

```