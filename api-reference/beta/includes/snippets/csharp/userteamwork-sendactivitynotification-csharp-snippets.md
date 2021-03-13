---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d45452c2f348637dc37e9af9109b02ef248e85d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
};

var activityType = "taskCreated";

var previewText = new ItemBody
{
    Content = "New Task Created"
};

var templateParameters = new List<KeyValuePair>()
{
    new KeyValuePair
    {
        Name = "taskId",
        Value = "Task 12322"
    }
};

await graphClient.Users["{user-id}"].Teamwork
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,null)
    .Request()
    .PostAsync();

```