---
title: 'team: sendActivityNotification'
description: Отправка уведомления веб-канала активности в области команды.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f4ad396d25ee20bd4adc5bf579925bbd4e8de1fd
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754063"
---
# <a name="team-sendactivitynotification"></a>team: sendActivityNotification
Пространство имен: microsoft.graph

Отправка уведомления веб-канала активности в области команды. Дополнительные сведения об отправке уведомлений и требованиях для этого см. в отправке уведомлений [о действиях Teams.](/graph/teams-send-activityfeednotifications)

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

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|topic|[teamworkActivityTopic](../resources/teamworkactivitytopic.md)|Тема уведомления. Указывает ресурс, о который идет речь.|
|activityType|String|Тип действия. Это должно быть объявлено в манифесте [приложения Teams.](/microsoftteams/platform/overview)|
|chainId|Int64|Необязательный элемент. Используется для переопределения предыдущего уведомления. Используйте то же самое `chainId` в последующих запросах для переопределения предыдущего уведомления.|
|previewText|[itemBody](../resources/itembody.md)|Предварительный просмотр текста уведомления. Microsoft Teams будет показывать только первые 150 символов.|
|templateParameters|Коллекция [keyValuePair](../resources/keyvaluepair.md)|Значения переменных шаблона, определенных в записи веб-канала активности, соответствующей `activityType` [манифесту приложения Teams.](/microsoftteams/platform/overview)|
|получатель;|[teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md)|Получатель уведомления. Поддерживаются только пользователи Azure AD. См. [также aadUserNotificationRecipient.](../resources/aadusernotificationrecipient.md) |

Следующие ресурсы поддерживаются при установке для свойства `source` **темы** значения `entityUrl` :

- [team](../resources/team.md)
- [channel](../resources/channel.md)
- [chatMesage](../resources/chatmessage.md)
- [teamsTab](../resources/teamstab.md)

> **Примечание.** URL-адрес сущности должен быть тем же или иным ресурсом команды в URL-адресе. Кроме того, приложение [Teams](/microsoftteams/platform/overview) должно быть установлено в команде.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a>Пример 1. Уведомление пользователя об ожидающих запросах на финансовое утверждение

В этом примере показано, как можно отправить уведомление веб-канала активности для команды. В этом примере владельцу команды сообщается об ожидающих запросах на финансовое утверждение.

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

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
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

### <a name="example-2-notify-a-user-about-a-channel-tab"></a>Пример 2. Уведомление пользователя о вкладке канала

Как и в предыдущем примере, в этом примере `entityUrl` используется для `topic` . Однако в этом примере ссылки на [вкладку](../resources/teamstab.md) в [канале.](../resources/channel.md) На вкладке размещена страница с состоянием резервирования в гостинице. При выборе уведомления пользователь перенаберется на вкладку, где он сможет проверить свое резервирование.

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

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a>Пример 3. Уведомление пользователя о событии с помощью настраиваемой темы

Как видно из предыдущих примеров, вы можете ссылаться на различные аспекты команды. Однако если вы хотите связать аспект, который не является частью команды или не представлен Microsoft Graph, или вы хотите настроить имя, вы можете настроить источник и передать для него настраиваемые `topic` `text` значения. `webUrl` требуется при установке `topic` для источника параметра `text` ..

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
