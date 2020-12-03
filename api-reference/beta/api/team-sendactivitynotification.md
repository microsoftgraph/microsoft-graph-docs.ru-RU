---
title: 'команда: Сендактивитинотификатион'
description: Отправка уведомления о канале активности в области действия команды.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6db256a71c17e4c940669aaf96f61f70285c8f3e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523415"
---
# <a name="team-sendactivitynotification"></a>команда: Сендактивитинотификатион
Пространство имен: microsoft.graph

Отправка уведомления о канале активности в области действия команды. Дополнительные сведения об отправке уведомлений и требованиях для этого можно найти в разделе [Отправка уведомлений о действиях в группах](/graph/teams-send-activityfeednotifications).

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
POST /teams/{teamId}/sendActivityNotification
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

Следующие ресурсы поддерживаются при задании `source` значения свойства **Topic** `entityUrl` следующим образом:

- [team](../resources/team.md)
- [channel](../resources/channel.md)
- [чатмесаже](../resources/chatmessage.md)
- [teamsTab](../resources/teamstab.md)

> **Примечание:** URL-адрес сущности должен быть таким же или дочерним ресурсом команды в URL-адресе. Кроме того, в команде должно быть установлено [приложение](/microsoftteams/platform/overview) Teams.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a>Пример 1: уведомить пользователя о предопределенном запросе на утверждение в финансах

В этом примере показано, как можно отправить уведомление веб-канала активности для команды. В этом примере владелец команды уведомляется о незавершенных запросах на утверждение в финансах.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
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

### <a name="example-2-notify-a-user-about-a-channel-tab"></a>Пример 2: уведомление пользователя о вкладке канала

Как и в предыдущем примере, в этом примере используется `entityUrl` для `topic` . Однако в этом примере показано, как создать ссылку на [вкладку](../resources/teamstab.md) в [канале](../resources/channel.md). На вкладке размещается страница, на которой пользователь находится в состоянии бронирования гостиницы. При выборе уведомления пользователь будет переходить на вкладку, где они могут проверить резервирование.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    },
    "activityType": "reservationUpdated",
    "previewText": {
        "content": "You have moved up the queue"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "reservationId",
            "value": "TREEE433"
        },
        {
            "name": "currentSlot",
            "value": "23"
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

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a>Пример 3: уведомление пользователя о событии с помощью настраиваемого раздела

Как показано в предыдущих примерах, вы можете ссылаться на различные аспекты команды. Тем не менее, если вы хотите создать ссылку на аспект, не являющийся частью команды или не представленный в Microsoft Graph, или вы хотите изменить имя, вы можете задать `topic` для `text` него значение и передать его настраиваемое значение. `webUrl` является обязательным, если задано значение `topic` source `text` .

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
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
