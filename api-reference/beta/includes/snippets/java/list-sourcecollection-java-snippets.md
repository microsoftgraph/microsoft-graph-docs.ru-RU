---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ea964406a89c5aef88b0d7714aeccb8fe93fef1a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776608"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISourceCollectionCollectionPage sourceCollections = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections()
    .buildRequest()
    .get();

```