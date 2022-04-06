---
title: Получение sharedWithChannelTeamInfo
description: Получение общего доступа к команде с каналом.
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: d2c82aa499e33a51f2b738328e23850f100833bf
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685294"
---
# <a name="get-sharedwithchannelteaminfo"></a>Получение sharedWithChannelTeamInfo
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение общего [доступа](../resources/sharedwithchannelteaminfo.md) к команде с [каналом](../resources/channel.md). Эта операция разрешена только для каналов со **значением membershipType**`shared`.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|ChannelMember.Read.All, ChannelMember.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|ChannelMember.Read.All, ChannelMember.ReadWrite.All |

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/channels/{channelId}/sharedWithTeams/{sharedWithChannelTeamInfoId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не поддерживает параметры запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и общий [объектWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_sharedwithchannelteaminfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/sharedWithTeams/893075dd-2487-5634-925f-022c42e20265
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedWithChannelTeamInfo"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
    "id": "2173de69-de69-2173-69de-732169de7321",
    "tenantId": "b3246f44-b4gb-4627-96c6-25b18fa2c910",
    "displayName": "Team contosso",
    "isHostTeam": true
  }
}
```

