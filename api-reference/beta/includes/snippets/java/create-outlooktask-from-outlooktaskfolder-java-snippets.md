---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 774dda002d1e691264477b9f2964f3826a0513f5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTask outlookTask = new OutlookTask();
outlookTask.subject = "Shop for dinner";
DateTimeTimeZone startDateTime = new DateTimeTimeZone();
startDateTime.dateTime = "2016-04-23T18:00:00";
startDateTime.timeZone = "Pacific Standard Time";
outlookTask.startDateTime = startDateTime;
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2016-04-25T13:00:00";
dueDateTime.timeZone = "Pacific Standard Time";
outlookTask.dueDateTime = dueDateTime;

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPXAAA=").tasks()
    .buildRequest()
    .post(outlookTask);

```