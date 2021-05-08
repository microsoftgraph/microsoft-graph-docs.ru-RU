---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a29ca75a6560f52525b9d71417f22584f29dae36
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241174"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdateCategory updateCategory = UpdateCategory.FEATURE;

String memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("String");
idsList.add("String");
idsList.add("String");

graphClient.admin().windows().updates().updatableAssets()
    .enrollAssetsById(UpdatableAssetEnrollAssetsByIdParameterSet
        .newBuilder()
        .withUpdateCategory(updateCategory)
        .withMemberEntityType(memberEntityType)
        .withIds(idsList)
        .build())
    .buildRequest()
    .post();

```