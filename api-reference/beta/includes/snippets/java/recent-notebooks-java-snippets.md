---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 82c000e87e535074efe305cb959c1e69657377a3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772494"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

INotebookGetrecentnotebooksCollectionPage getrecentnotebooks = graphClient.me().onenote().notebooks()
    .getrecentnotebooks(true)
    .buildRequest()
    .get();

```