---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bf1ef23ed3d57648ddc0404b6ee6c7edff1a7e0e0b6e8089cbb8f31210ddb050
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57204512"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSetCollectionPage reviewSets = graphClient.compliance().ediscovery().cases("{caseId}").reviewSets()
    .buildRequest()
    .get();

```