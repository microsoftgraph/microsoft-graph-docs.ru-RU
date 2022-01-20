---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ac57c7b2d3817170e86e14738b7b6a05c1e211c2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114178"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskCollectionPage tasks = graphClient.me().tasks().lists("AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm").tasks()
    .buildRequest()
    .get();

```