---
title: Ответы Graph API безопасности
description: Ошибки в API Graph безопасности возвращаются с помощью стандартного кода состояния частичного контента HTTP 206 и доставляются через предупреждающий заголовок.
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 674ccf9817d01f48a0db40906ba2cfd656ff3dfe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080571"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Ответы Graph API безопасности

Пространство имен: microsoft.graph

Ошибки в API Graph безопасности возвращаются с помощью стандартного кода состояния частичного контента HTTP 206 и доставляются через предупреждающий заголовок.

## <a name="errors"></a>Ошибки

API Graph безопасности — это федератная служба, которая получает несколько ответов от всех поставщиков данных. При получении ошибки HTTP в API Graph безопасности Майкрософт будет отсылаться предупреждающий заголовок в следующем формате:
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Этот предостережение отправляется клиентам только в том случае, если один из поставщиков данных возвращает код ошибки, не 2xx или 404. Например:

- HttpStatusCode.Forbidden (403) может быть возвращен, если доступ к ресурсу не предоставлен.
- Если поставщик разовое время, в загоне предупреждения возвращается httpStatusCode.GatewayTimeout (504).
- Если происходит внутренняя ошибка поставщика, в загонщике предупреждения используется httpStatusCode.InternalServerError (500).

Если поставщик данных возвращает 2xx или 404, он не отображается в загонах предупреждений, так как эти коды должны быть успешно или если данные не найдены соответственно. В федератной системе ожидается, что 404 не найдены, так как много раз данные известны только одному или нескольким поставщикам, но не всем.

## <a name="example"></a>Пример

Пользователь просит `security/alerts/{alert_id}` .

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

Так как 404 и 200 являются ожидаемыми условиями, в загонах предупреждения содержится следующее:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Примечание:** Каждый заглавный элемент HTTP — это коллекция подитемов, поэтому пользователи могут перенаценять заготку Warning и проверять все элементы.

## <a name="threat-indicator-bulk-action-errors"></a>Ошибки массовых действий индикатора угроз

Массовые действия (создание, обновление, удаление) могут создавать два различных кода потенциальных ошибок:

- Код ошибки 400 указывает, что предоставленный орган имел ошибку во время сериализации.
- Код ошибки 206 указывает, что одно или несколько массовых действий не удалось при его федерате поставщике. Ответ будет содержать данные об успехах и ошибках отдельных поставщиков для каждого индикатора разведки угроз. В отличие от оповещений, вся потенциальная информация об ошибках будет содержаться в теле ответа на массовые действия [tiIndicator.](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) [](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts)

## <a name="constraints"></a>Ограничения

Параметр `$top` запроса OData имеет ограничение в 1000 оповещений. В первый запрос GET рекомендуется включить только параметр `$top`, но не параметр `$skip`. Для разбивки на страницы можно использовать параметр `@odata.nextLink`. Если требуется применить параметр `$skip`, он имеет ограничение в 500 оповещений. Например, `/security/alerts?$top=10&$skip=500` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=501` вернет код отклика `400 Bad Request`. Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).

Обходным путем для этого ограничения является использование параметра запроса OData с объектом оповещения из API безопасности Microsoft Graph, используя и заменяя значение dateTime последним `$filter` `eventDateTime` `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` (1500-м) оповещением. Вы также можете установить диапазон `eventDateTime` для ; например, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z` .

## <a name="see-also"></a>См. также

Если у вас возникли проблемы с авторизацией, см. авторизацию и [API Graph microsoft.](/graph/security-authorization)


