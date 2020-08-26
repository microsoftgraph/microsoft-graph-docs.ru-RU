---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ff5b404561e43f0aa1b61c14585c12c5a50ee61
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873913"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage search = graphClient.me().drive()
    .search("Contoso Project")
    .buildRequest()
    .get();

```