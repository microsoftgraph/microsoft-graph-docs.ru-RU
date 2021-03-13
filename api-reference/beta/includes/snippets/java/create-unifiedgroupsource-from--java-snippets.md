---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cd27f6825ed45bb250efea2379faec4a69cbfa9d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773223"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSource unifiedGroupSource = new UnifiedGroupSource();
unifiedGroupSource.additionalDataManager().put("group@odata.bind", new JsonPrimitive("/groups/000044f9-47c8-4a87-bccf-291fbf006a54"));
unifiedGroupSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.compliance().ediscovery().cases("{caseId}").custodians("{custodianId}").unifiedGroupSources()
    .buildRequest()
    .post(unifiedGroupSource);

```