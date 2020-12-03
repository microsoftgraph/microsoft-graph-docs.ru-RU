---
title: 'чат: Сендактивитинотификатион'
description: Отправка уведомления о канале активности в области разговора.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76598572ebca1421770de5a298f46fdedc30a0c9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522001"
---
# <a name="chat-sendactivitynotification"></a>чат: Сендактивитинотификатион
Пространство имен: microsoft.graph

Отправка уведомления о канале активности в области разговора. Дополнительные сведения об отправке уведомлений и требованиях для этого можно найти в разделе [Отправка уведомлений о действиях в группах](/graph/teams-send-activityfeednotifications).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamsActivity.Send|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|TeamsActivity.Send|

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
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|topic|[теамворкактивититопик](../resources/teamworkactivitytopic.md)|Тема уведомления. Указывает ресурс, о котором идет речь.|
|activityType|String|Тип действия. Он должен быть объявлен в [манифесте приложения Teams](/microsoftteams/platform/overview).|
|чаинид|Int64|Необязательный параметр. Используется для переопределения предыдущего уведомления. Используйте одно и то же `chainId` в последующих запросах для переопределения предыдущего уведомления.|
|previewText|[itemBody](../resources/itembody.md)|Предварительный просмотр текста уведомления. Microsoft Teams будет показывать только первые 150 символов.|
|темплатепараметерс|Коллекция [keyValuePair](../resources/keyvaluepair.md)|Значения для переменных шаблона, определенных в записи веб-канала активности, соответствующей `activityType` [манифесту приложения Teams](/microsoftteams/platform/overview).|
|получатель;|[теамворкнотификатионреЦипиент](../resources/teamworknotificationrecipient.md)|Получатель уведомления. Поддерживаются только пользователи Azure AD. См. также [аадусернотификатионреЦипиент](../resources/aadusernotificationrecipient.md). |

Следующие ресурсы поддерживаются при задании `source` значения свойства **Topic** `entityURL` следующим образом:

- [chat](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

> **Примечание:** URL-адрес сущности должен быть таким же, как или дочерний ресурс чата в URL-адресе. Кроме того, [приложение Teams](/microsoftteams/platform/overview) должно быть установлено в чате.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>Пример 1: уведомление пользователя о задаче, созданной в чате

В этом примере показано, как можно отправить уведомление веб-канала активности для новой задачи, созданной в чате. Более подробную информацию можно узнать в статье [Отправка уведомлений о действиях в группах](/graph/teams-send-activityfeednotifications).

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
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
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-java-snippets.md)]
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

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a>Пример 2: уведомление пользователя о необходимости утверждения в сообщении чата

Как и в предыдущем примере, в этом примере используется `entityUrl` для `topic` . Однако в этом случае он связывается с сообщением в чате. Сообщение может содержать карточку с кнопкой утверждения на ней.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
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

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a>Пример 3: уведомление пользователя о событии относительно чата

Как показано в предыдущих примерах, вы можете ссылаться на различные аспекты разговора. Тем не менее, если вы хотите создать ссылку на аспект, не входящий в чат или не представленный в Microsoft Graph, можно установить для него в качестве источника `topic` `text` значение и передать его настраиваемое значение. Кроме того, `webUrl` требуется, если для параметра Source задано значение `topic` `text` .

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
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

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
