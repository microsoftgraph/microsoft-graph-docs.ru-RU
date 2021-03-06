---
title: Ответы на ошибки API безопасности Microsoft Graph
description: Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: c36cf3be4cf24a2831918acd994a36bbcfc9e489
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988928"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Ответы на ошибки API безопасности Microsoft Graph

Пространство имен: microsoft.graph

Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.

## <a name="errors"></a>Ошибки

API безопасности Microsoft Graph — это Федеративная служба, которая получает несколько ответов от всех поставщиков данных. При получении сообщения об ошибке HTTP с помощью API безопасности Microsoft Graph он отправляет заголовку предупреждения в следующем формате:
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Этот заголовок предупреждения отправляется обратно только клиентам, когда один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404. Например:

- HttpStatusCode. запрещено (403) может быть возвращено, если доступ к ресурсу не предоставляется.
- Если время ожидания поставщика истекло, в заголовке предупреждения возвращается HttpStatusCode. Гатевайтимеаут (504).
- Если происходит ошибка внутреннего поставщика, в заголовке предупреждения используется HttpStatusCode. Интерналсервереррор (500).

Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждения, так как эти коды являются ожидаемыми для успешного выполнения или когда данные не были найдены соответственно. В федеративной системе ожидается 404, но ожидается, что данные не будут найдены одному или нескольким, но не всем, поставщикам.

## <a name="example"></a>Пример

Пользователь запрашивает `security/alerts/{alert_id}` .

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

Так как 404 и 200, ожидаемые условия, заголовок предупреждения содержит следующие сведения:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Примечание:** Каждый заголовок HTTP является коллекцией подэлементов, поэтому пользователи могут перечислить заголовок предупреждения и проверить все элементы.

## <a name="threat-indicator-bulk-action-errors"></a>Ошибки массовых действий индикатора угроз

Групповые действия (создание, обновление, удаление) могут создавать два различных возможных кода ошибки:

- Код ошибки 400 указывает на то, что во время сериализации получено сообщение об ошибке.
- Код ошибки 206 указывает на то, что одно или несколько массовых действий завершились неудачно, если они были объединены со своим поставщиком. Ответ будет содержать сведения об успешном выполнении и ошибках отдельных поставщиков для каждого индикатора логики операций с угрозами. В отличие от [оповещений](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), все возможные сведения об ошибках будут содержаться в теле ответа для массовых действий [тииндикатор](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) .

## <a name="constraints"></a>Провероч

`$top`Параметр запроса OData имеет лимит в 1000 оповещений. В первый запрос GET рекомендуется включить только параметр `$top`, но не параметр `$skip`. Для разбивки на страницы можно использовать параметр `@odata.nextLink`. Если требуется применить параметр `$skip`, он имеет ограничение в 500 оповещений. Например, `/security/alerts?$top=10&$skip=500` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=501` вернет код отклика `400 Bad Request`. Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).

Чтобы устранить это ограничения, используйте `$filter` параметр запроса OData с `eventDateTime` объектом Alert из API безопасности Microsoft Graph, используя `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` и заменив значение DateTime на Последнее (1500th) оповещение. Кроме того, можно задать диапазон для, например `eventDateTime` , `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z` .

## <a name="see-also"></a>См. также

Если у вас возникли проблемы с авторизацией, обратитесь к разделу [авторизация и API безопасности Microsoft Graph](/graph/security-authorization).


