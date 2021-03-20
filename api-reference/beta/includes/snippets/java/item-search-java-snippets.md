---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7cbd5a6d6d500806878e3cd213211522b8d26848
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970022"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemSearchCollectionPage search = graphClient.me().drive().root()
    .search(DriveItemSearchParameterSet
        .newBuilder()
        .withQ("Contoso Project")
        .build())
    .buildRequest()
    .get();

```