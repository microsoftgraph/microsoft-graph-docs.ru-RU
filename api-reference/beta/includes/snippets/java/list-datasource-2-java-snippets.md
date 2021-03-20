---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4524b47cf003699f32d52dceb916cdf1d5df0c2f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952131"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDataSourceCollectionWithReferencesPage custodianSources = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}").custodianSources()
    .buildRequest()
    .get();

```