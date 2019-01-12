---
title: Сообщения об ошибках API безопасности Microsoft Graph
description: Ошибки в API-Интерфейс безопасности Microsoft Graph возвращаются с помощью стандартных код состояния HTTP 206 Частичное контента и являются через заголовок предупреждения.
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 52b7c375bd3e0c6a367f1150a21bb96ef84437ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921431"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Сообщения об ошибках API безопасности Microsoft Graph

Ошибки в API-Интерфейс безопасности Microsoft Graph возвращаются с помощью стандартных код состояния HTTP 206 Частичное контента и являются через заголовок предупреждения.

## <a name="errors"></a>Ошибки

API-Интерфейс безопасности Microsoft Graph — федеративных служба, которая получает несколько ответов от всех поставщиков данных. При получении ошибки HTTP с API-Интерфейс безопасности Microsoft Graph возвращается предупреждение заголовка в следующем формате:<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Этот заголовок предупреждение только отправляется обратно клиентов при один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404. Пример:

- HttpStatusCode.Forbidden (403) может быть возвращено, если не предоставляется доступ к ресурсу.
- Если поставщик времени ожидания, HttpStatusCode.GatewayTimeout (504) возвращается в заголовке предупреждения.
- Если происходит ошибка внутреннего поставщика HttpStatusCode.InternalServerError (500) используется в заголовке предупреждения.

Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждение так как эти коды для успеха или когда данные не найдены соответственно. В системе с федеративным 404 не найден ожидается как количество раз данные известно только один или несколько, но не для всех поставщиков.

## <a name="example"></a>Пример

Пользователь запрашивает `security/alerts/{alert_id}`.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Так как 404 и 200 ожидаемых условиях, предупреждение заголовка содержит следующие элементы:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Примечание:** Каждого заголовка HTTP — это коллекция элементов, чтобы пользователи могли предупреждение заголовок перечислить и проверить все элементы.

## <a name="constraints"></a>Ограничения

`$top` Параметр запроса OData для которого настроено ограничение 1000 оповещений и сочетание `$top`  +  `$skip` параметров не может превышать 6000 оповещения запросов OData. Например `/security/alerts?$top=10&$skip=5990` возвращает `200 OK` код ответа, но `/security/alerts?$top=10&$skip=5991` возвращает `400 Bad Request` код ответа.

Обходной предела является использование `$filter` параметр запроса OData с `eventDateTime` оповещения сущности из Microsoft Graph безопасности API, с помощью `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` и замените значение даты и времени последнего предупреждения (6000th). Можно также задать диапазон для `eventDateTime`; например *alerts?$ фильтра = Дата и время **gt** 2018-11 -**11**T00:00:00.000Z & Дата и время **lt** 2018-11 -**12**T00:00:00.000Z*

## <a name="see-also"></a>См. также

Если у вас возникли неполадки с авторизации, видеть [авторизации и API -Интерфейс Microsoft Graph безопасности](/graph/security-authorization).
