---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0e1a4698f3f88273bf493eca5205c390eae73ef1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971826"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskCollectionPage tasks = graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPWAAA=").tasks()
    .buildRequest()
    .get();

```