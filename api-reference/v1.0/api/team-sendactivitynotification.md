---
title: 'команда: sendActivityNotification'
description: Отправьте уведомление о канале действий в области группы.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc50e9ca132b295f000a707a9fc3280bef2bb6e6eb564aca0ae69020b1d2a498
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57372081"
---
# <a name="team-sendactivitynotification"></a>команда: sendActivityNotification
Пространство имен: microsoft.graph

Отправьте уведомление о канале действий в области группы. Дополнительные сведения об отправке уведомлений и требованиях к этому см. в Teams [действия.](/graph/teams-send-activityfeednotifications)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamsActivity.Send|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
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
|topic|[teamworkActivityTopic](../resources/teamworkactivitytopic.md)|Тема уведомления. Указывает обсуждаемый ресурс.|
|activityType|String|Тип действия. Это должно быть объявлено в [манифесте Teams приложения](/microsoftteams/platform/overview).|
|chainId|Int64|Необязательное свойство. Используется для переопределения предыдущего уведомления. Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.|
|previewText|[itemBody](../resources/itembody.md)|Предварительный текст уведомления. Microsoft Teams только первые 150 символов.|
|templateParameters|Коллекция [keyValuePair](../resources/keyvaluepair.md)|Значения переменных шаблонов, определенных в записи ленты действий, соответствующие манифесту `activityType` [Teams приложения.](/microsoftteams/platform/overview)|
|получатель;|[teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md)|Получатель уведомления. Поддерживаются только пользователи Azure AD. См. [также aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md). |

При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityUrl` ресурсы:

- [team](../resources/team.md)
- [channel](../resources/channel.md)
- [chatMesage](../resources/chatmessage.md)
- [teamsTab](../resources/teamstab.md)

> **Примечание:** URL-адрес объекта должен быть одним и тем же или детским ресурсом группы в URL-адресе. Кроме того, [Teams приложение должно](/microsoftteams/platform/overview) быть установлено в команде.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a>Пример 1. Уведомление пользователя о ожидающих запросах на утверждение финансирования

В этом примере показано, как можно отправить уведомление о канале действий для группы. В этом примере владелец группы сообщает о ожидающих запросах на утверждение финансирования.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}"
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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

Как и в предыдущем примере, в этом примере `entityUrl` используется `topic` для . Однако в этом примере ссылки на [вкладку](../resources/teamstab.md) в [канале](../resources/channel.md). На вкладке размещена страница, показывающая пользователю состояние бронирования в отеле. Выбор уведомления будет принимать пользователя на вкладке, где он может проверить свое бронирование.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
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

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a>Пример 3. Уведомление пользователя о событии с использованием настраиваемой темы

Как повествуют в предыдущих примерах, вы можете ссылаться на различные аспекты команды. Однако если вы хотите связаться с аспектом, который не является частью команды или не представлен Корпорацией Майкрософт Graph, или вы хотите настроить имя, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него. `webUrl` требуется при настройке `topic` источника `text` для .

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
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
