---
title: Перечисление всех каналов
description: Получение списка каналов в этой команде или общий доступ к этой команде (входящие каналы).
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 4f5f025062089d3550fe8f2212b353757059bd12
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685322"
---
# <a name="list-allchannels"></a>Перечисление всех каналов
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка каналов [в этой](../resources/channel.md) [команде или](../resources/team.md) общий доступ к этой [команде](../resources/team.md) (входящие каналы).

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
GET /teams/{teamsId}/allChannels
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

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию [объектов канала](../resources/channel.md) в тексте отклика. Ответ также включает свойство **@odata.id** , которое можно использовать для доступа к каналу и выполнения других операций в [объекте](../resources/channel.md) канала.

> [!Note]
> В настоящее время вызов URL-адреса, **возвращаемого свойством @odata.id** , завершается сбоем для общих каналов между клиентами. Эту проблему можно решить, если удалить `/tenants/{tenant-id}` часть из URL-адреса перед вызовом этого API. Дополнительные сведения см[. в разделе "Известные проблемы с microsoft Graph](/graph/known-issues#unable-to-access-a-cross-tenant-shared-channel-when-the-request-url-contains-tenantscross-tenant-id)".

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
      "displayName": "Shared channel from Contosso",
      "membershipType": "shared",
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```


### <a name="example-2-list-all-shared-channels"></a>Пример 2. Вывод списка всех общих каналов

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
      "displayName": "Shared channel from Contosso",
      "membershipType": "shared",
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```

