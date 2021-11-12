---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e174e9598e07edd14ba81f618dd43fbedf3429e1379ccc87d5077f5b2370f6b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138378"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskCollectionPage tasks = graphClient.print().taskDefinitions("92d72a3d-cad7-4809-8924-43833282b079").tasks()
    .buildRequest()
    .get();

```