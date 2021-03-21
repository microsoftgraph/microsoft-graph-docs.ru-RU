---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b32658c5304b288b6bfbbdd2d80b8e9373fcc4e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975456"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlowCollectionPage b2xUserFlows = graphClient.identity().b2xUserFlows()
    .buildRequest()
    .get();

```