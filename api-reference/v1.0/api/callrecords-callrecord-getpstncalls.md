---
title: 'callRecord: getPstnCalls'
description: Получить журнал вызовов PSTN.
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: eaa0f1e4c61b78c19b8043ff24fd6d222aa52df7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056862"
---
# <a name="callrecord-getpstncalls"></a>callRecord: getPstnCalls

Пространство имен: microsoft.graph.callRecords

Получите журнал вызовов PSTN в качестве коллекции записей [pstnCallLogRow.](../resources/callrecords-pstncalllogrow.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | CallRecord-PstnCalls.Read.All, CallRecords.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.
В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.

|Параметр|Тип|Описание|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|Начало диапазона времени для запроса. UTC включительно.<br/>Диапазон времени зависит от времени начала вызова.|
|toDateTime|DateTimeOffset|Конец диапазона времени для запроса. UTC включительно.|

> [!IMPORTANT]
> Значения **fromDateTime** и **toDateTime** не могут быть больше диапазона дат в 90 дней.

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код ответа и коллекцию записей `200 OK` [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) в тексте ответа.
  
Если в диапазоне дат более 1000 записей, тело также включает URL-адрес для запроса следующей страницы записей `@odata.NextLink` вызовов. Последняя страница в диапазоне дат не имеет `@odata.NextLink` . Дополнительные сведения см. [в Graph microsoft Graph в приложении.](/graph/paging)

## <a name="example"></a>Пример

В следующем примере показано получение коллекции записей для вызовов PSTN, которые произошли в указанном диапазоне дат. Ответ включает в себя список записей в этом первом ответе и получения записей за пределами первых `"@odata.count": 1000` `@odata.NextLink` 1000. Для читаемости в ответе показана только коллекция из 1 записи. Предположим, что в этом диапазоне дат более 1000 вызовов.

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/callrecord-getpstncalls-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/callrecord-getpstncalls-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/callrecord-getpstncalls-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/callrecord-getpstncalls-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.pstnCallLogRow)"
}
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.callRecords.pstnCallLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9c4984c7-6c3c-427d-a30c-bd0b2eacee90",
            "callId": "1835317186_112562680@61.221.3.176",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:08.2589935Z",
            "endDateTime": "2019-11-01T00:03:47.2589935Z",
            "duration": 219,
            "charge": 0.00,
            "callType": "user_in",
            "currency": "USD",
            "calleeNumber": "+1234567890",
            "usageCountryCode": "US",
            "tenantCountryCode": "US",
            "connectionCharge": 0.00,
            "callerNumber": "+0123456789",
            "destinationContext": null,
            "destinationName": "United States",
            "conferenceId": null,
            "licenseCapability": "MCOPSTNU",
            "inventoryType": "Subscriber",
            "operator": "Microsoft",
            "callDurationSource": "microsoft"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>См. также

* [Microsoft Teams отчет об использовании PSTN](/microsoftteams/teams-analytics-and-reports/pstn-usage-report).
* [Отчет о прямой маршрутике в Microsoft Graph](callrecords-callrecord-getdirectroutingcalls.md).
