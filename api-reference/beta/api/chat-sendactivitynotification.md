---
title: 'чат: sendActivityNotification'
description: Отправьте уведомление о канале действий в области чата.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1df0fdd33d02269f2595d40515ad17d7b48210c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348857"
---
# <a name="chat-sendactivitynotification"></a>чат: sendActivityNotification
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отправьте уведомление о канале действий в области чата. Дополнительные сведения об отправке уведомлений и требованиях для этого см. в Teams [действий](/graph/teams-send-activityfeednotifications).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamsActivity.Send|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|TeamsActivity.Send.Chat*, TeamsActivity.Send|

>**Примечание:** Разрешения, помеченные *, [используют разрешение, определенное для ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|topic|[teamworkActivityTopic](../resources/teamworkactivitytopic.md)|Тема уведомления. Указывает обсуждаемый ресурс.|
|activityType|String|Тип действия. Это должно быть объявлено в [манифесте Teams приложения](/microsoftteams/platform/overview).|
|chainId|Int64|Необязательный параметр. Используется для переопределения предыдущего уведомления. Используйте то же самое `chainId` в последующих запросах для переопределения предыдущего уведомления.|
|previewText|[itemBody](../resources/itembody.md)|Предварительный текст уведомления. Microsoft Teams только первые 150 символов.|
|templateParameters|Коллекция [keyValuePair](../resources/keyvaluepair.md)|Значения для переменных шаблонов, определенных в записи `activityType` ленты действий, соответствующие манифесту [Teams приложения](/microsoftteams/platform/overview).|
|получатель;|[teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md)|Получатель уведомления. См. [также aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) и [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md). |

При настройке `source` значения свойства темы для следующих ресурсов  поддерживаются `entityURL`следующие ресурсы:

- [chat](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

> **Примечание:** URL-адрес объекта должен быть таким же, как или детский ресурс чата в URL-адресе. Кроме того, [Teams приложение должно](/microsoftteams/platform/overview) быть установлено в чате.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>Пример 1. Уведомление пользователя о задаче, созданной в чате

В этом примере показано, как можно отправить уведомление о ленте действий для новой задачи, созданной в чате. Дополнительные сведения см. в [Teams уведомлений об активности](/graph/teams-send-activityfeednotifications).

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_1"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chat-sendactivitynotification-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/chat-sendactivitynotification-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-approval-needed-in-a-chat-message"></a>Пример 2. Уведомление пользователя об утверждении, необходимом в сообщении чата

Как и в предыдущем примере, в этом примере используется `entityUrl` для .`topic` Однако в этом случае он связывается с сообщением в чате. В сообщении может быть карточка с кнопкой утверждения.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_2"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "Deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "approvalTaskId",
            "value": "2020AAGGTAPP"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chat-sendactivitynotification-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/chat-sendactivitynotification-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-approval-needed-in-a-chat-message-using-user-principal-name"></a>Пример 3. Уведомление пользователя об утверждении, необходимом в сообщении чата с использованием основного имени пользователя

Как и в предыдущем примере, в этом примере используется `entityUrl` для .`topic` Однако в этом случае он связывается с сообщением в чате. В сообщении может быть карточка с кнопкой утверждения.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_upn"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "Deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "jacob@contoso.com"
    },
    "templateParameters": [
        {
            "name": "approvalTaskId",
            "value": "2020AAGGTAPP"
        }
    ]
}
```


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-a-user-about-an-event-in-relation-to-a-chat"></a>Пример 4. Уведомление пользователя о событии по отношению к чату

Как показано в предыдущих примерах, вы можете связаться с различными аспектами чата. Однако, если вы хотите связаться с аспектом, который не является частью чата или не представлен Microsoft Graph, `topic` `text` вы можете установить источник и передать в настраиваемом значении для него. Кроме того, `webUrl` требуется при настройке `topic` источника для `text`.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_3"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "deploymentApprovalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chat-sendactivitynotification-3-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/chat-sendactivitynotification-3-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-chat-members-about-a-task-created-in-a-chat"></a>Пример 5. Уведомление участников чата о задаче, созданной в чате.

В этом примере показано, как можно отправить уведомление о канале действий всем участникам чата. Этот пример похож на предыдущие примеры. Однако в этом случае `recipient` это [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md). Обратите внимание, `chatId` что указанный в должен `recipient` соответствовать указанному `chatId` в URL-адресе запроса.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_4"
}
-->

``` http
POST https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
        "chatId": "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chat-sendactivitynotification-4-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/chat-sendactivitynotification-4-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
