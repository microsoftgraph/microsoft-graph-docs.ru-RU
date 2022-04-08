---
title: Список всех каналов
description: Получите список каналов в этой команде или общих с этой командой (входящие каналы).
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 77332d239310ab4552d724362c19d770d6f1d471
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704205"
---
# <a name="list-allchannels"></a>Список всех каналов
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получить список [каналов](../resources/channel.md) в этой [команде](../resources/team.md) или общих с этой[командой](../resources/team.md) (входящие каналы).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись) | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All |


> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/allChannels
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter` и `$select` для настройки отклика.

### <a name="use-select-for-better-performance"></a>Использование $select для повышения производительности
Заполнение свойств **email** и **moderationSettings** для канала является затратной операцией, снижающей производительность. Используйте `$select`, чтобы исключить свойства **email** и **moderationSettings** для повышения производительности.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ каналов ](../resources/channel.md) в тексте отклика. Ответ также включает свойство **@odata.id**, которое можно использовать для доступа к каналу и запуска других операций с [каналом](../resources/channel.md).

> [!Note]
> Сейчас при запросе URL-адреса, возвращенного из свойства **@odata.id** найти общие каналы между клиентами, не удается. Эту проблему можно устранить, удалив часть `/tenants/{tenant-id}` из URL-адреса перед вызовом этого API. Подробнее см.[Известные проблемы с Microsoft Graph](/graph/known-issues#unable-to-access-a-cross-tenant-shared-channel-when-the-request-url-contains-tenantscross-tenant-id).

## <a name="examples"></a>Примеры

### <a name="example-1-list-all-channels"></a>Пример 1. Список всех каналов

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_all_channel"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/allChannels
```


#### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
       "@odata.id": "https://graph.microsoft.com/beta/tenants/b3246f44-b4gb-4627-96c6-25b18fa2c910/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
      "membershipType": "standard",
      "tenantId": "b3246f44-b4gb-4627-96c6-25b18fa2c910"
    },
    {
       "@odata.id": "https://graph.microsoft.com/beta/tenants/b3246f44-b4gb-5678-96c6-25b18fa2c910/teams/893075dd-5678-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv",
      "id": "19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "Shared channel from Contoso",
      "membershipType": "shared",
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```


### <a name="example-2-list-all-shared-channels"></a>Пример 2. Список всех общих каналов

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_all_shared_channel"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/allChannels?$filter=membershipType eq 'shared'
```


#### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
       "@odata.id": "https://graph.microsoft.com/beta/tenants/b3246f44-b4gb-5678-96c6-25b18fa2c910/teams/893075dd-5678-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv",
      "id": "19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "Shared channel from Contoso",
      "membershipType": "shared",
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```

