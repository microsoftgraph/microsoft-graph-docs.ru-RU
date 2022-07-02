---
title: 'deletedTeam: getAllMessages'
description: Извлечение всех сообщений из всех каналов в удаленной команде.
author: agnesliu
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ddb94c35b00a88041004d01567d572d157af84a9
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578145"
---
# <a name="deletedteam-getallmessages"></a>deletedTeam: getAllMessages
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение всех [сообщений](../resources/chatmessage.md) из всех [каналов](../resources/channel.md) в [удаленной команде](../resources/deletedteam.md), включая текстовые, аудио и видеосообщения.

Дополнительные сведения об использовании API экспорта Microsoft Teams для экспорта содержимого см. в статье [Экспорт содержимого с помощью API экспорта Microsoft Teams](/microsoftteams/export-teams-content).

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Не поддерживается.|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|ChannelMessage.Read.All|

> [!NOTE]
> Перед вызовом этого API с разрешениями приложения необходимо запросить доступ. Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Вы можете использовать параметр запроса `model`, который поддерживает значения `A` и `B`, в зависимости от предпочитаемой [модели лицензирования и оплаты](/graph/teams-licenses), как показано в следующих примерах.  

```http
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages?model=A
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages?model=B
```

Если параметр `model` не указан, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

Этот метод поддерживает параметр запроса [$top](/graph/query-parameters#top-parameter) для управления количеством элементов на отклик и параметр запроса [$filter](/graph/query-parameters#filter-parameter) с помощью запроса диапазона **dateTime** в **lastModifiedDateTime**. Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения эта функция возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "deletedteamthis_getallmessages"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/deletedTeams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teamwork/deletedTeams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1616990417393",
            "replyToId": null,
            "etag": "1616990417393",
            "messageType": "message",
            "createdDateTime": "2021-03-29T04:00:17.393Z",
            "lastModifiedDateTime": "2021-03-29T04:00:17.393Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3Ad5d2708d408c41d98424c1c354c19db3%40thread.tacv2/1616990417393?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990417393&parentMessageId=1616990417393",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test message"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:d5d2708d408c41d98424c1c354c19db3@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

