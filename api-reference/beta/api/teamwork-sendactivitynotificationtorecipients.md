---
title: 'teamwork: sendActivityNotificationToRecipients'
description: Массовое отправка уведомлений в веб-канале действий нескольким пользователям.
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc0135fcbd7508a435e562c4b2c96cf68da09124
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695685"
---
# <a name="teamwork-sendactivitynotificationtorecipients"></a>teamwork: sendActivityNotificationToRecipients

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отправка уведомлений веб-канала действий нескольким пользователям в пакетном режиме. 

Дополнительные сведения об отправке уведомлений и требованиях для этого см. в статье [Teams действий](/graph/teams-send-activityfeednotifications).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | TeamsActivity.Send                          |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | TeamsActivity.Send                          |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /teamwork/sendActivityNotificationToRecipients
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тело запроса добавьте параметры в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

| Параметр          | Тип                                                         | Описание                                                  |
| :----------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| topic              | [teamworkActivityTopic](../resources/teamworkactivitytopic.md) | Раздел уведомления. Указывает ресурс, о котором говорят. |
| activityType       | String                                                       | Тип действия. Он должен быть объявлен в [манифесте Teams приложения](/microsoftteams/platform/overview). |
| chainId            | Int64                                                        | Необязательно. Используется для переопределения предыдущего уведомления. Используйте то же самое `chainId` в последующих запросах, чтобы переопределить предыдущее уведомление. |
| previewText        | [itemBody](../resources/itembody.md)                         | Предварительный просмотр текста уведомления. Microsoft Teams будут отображаться только первые 150 символов. |
| templateParameters | Коллекция [keyValuePair](../resources/keyvaluepair.md)      | Значения переменных шаблона, определенных в записи веб-канала `activityType` действий, соответствующей Teams [манифеста приложения](/microsoftteams/platform/overview). |
| teamsAppId         | String                                                       | Необязательно. Teams идентификатор приложения Teams, связанного с уведомлением. Используется для устранения неоднозначности установленных приложений, если для одного пользователя-получателя установлено несколько приложений с одинаковым Azure AD идентификатором приложения. |
| recipients         | [Коллекция teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md) | Получатели уведомления. Поддерживаются только получатели [типа aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) . В одном запросе существует верхний предел в 100 получателей. |

Следующий ресурс поддерживается при установке `source` значения свойства **раздела** в следующее `entityUrl`:

- [teamsCatalogApp](../resources/teamscatalogapp.md)

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

## <a name="examples"></a>Примеры

### <a name="example-1-notify-multiple-users-about-pending-finance-approval-requests"></a>Пример 1. Уведомление нескольких пользователей об ожидающих запросах на утверждение финансовых данных

В следующем примере показано, как массово отправлять уведомления в веб-канале действий нескольким пользователям. В этом примере несколько заинтересованных лиц уведомляют об ожидающих запросах на утверждение финансовых данных.

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients_1"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ],
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
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
HTTP/1.1 202 Accepted
```

### <a name="example-2-notify-multiple-users-about-an-event-using-a-custom-topic"></a>Пример 2. Уведомление нескольких пользователей о событии с помощью пользовательского раздела

Если вы хотите связать аспект, который не представлен Microsoft Graph, или настроить имя, `topic` `text` можно задать источник и передать для него пользовательское значение. `webUrl` является обязательным при использовании источника `topic` в качестве `text`.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients_2"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
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
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ],
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ]
}
```

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false
}
-->


``` http
HTTP/1.1 202 Accepted
```
