---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b26b4b85a9b9ca538bc735c39eb15703577ead707f89b8ba7fa00376cd9076a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57258968"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollectionCollectionPage sourceCollections = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections()
    .buildRequest()
    .get();

```