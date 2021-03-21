---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d77f2a405c0e5603cad64c8bbbcaa9f2a400c039
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970919"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = new OutlookTaskFolder();
outlookTaskFolder.name = "Volunteer";

graphClient.me().outlook().taskFolders()
    .buildRequest()
    .post(outlookTaskFolder);

```