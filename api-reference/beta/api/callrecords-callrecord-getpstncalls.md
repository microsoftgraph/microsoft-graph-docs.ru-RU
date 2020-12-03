---
title: 'Каллрекорд: Жетпстнкаллс'
description: Получение журнала звонков PSTN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cb15b70a023fcdf9731b67704329e7dc0d212cc8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563187"
---
# <a name="callrecord-getpstncalls"></a>Каллрекорд: Жетпстнкаллс

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение журнала вызовов PSTN в виде коллекции записей [пстнкалллогров](../resources/callrecords-pstncalllogrow.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | CallRecords.Read.All |

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
|фромдатетиме|DateTimeOffset|Начало диапазона времени для запроса. UTC, включительно.<br/>Диапазон времени основан на времени начала вызова.|
|тодатетиме|DateTimeOffset|Конец диапазона времени для запроса. UTC, включительно.|

> [!IMPORTANT]
> \* Значения **фромдатетиме** и **тодатетиме** не могут превышать диапазон дат 90 дней.

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="response"></a>Отклик

В случае успешного выполнения эта функция возвращает `200 OK` код отклика и коллекцию записей [пстнкалллогров](../resources/callrecords-pstncalllogrow.md) в тексте отклика.
  
Если в диапазоне дат больше 1000 записей, в тексте также включается `@odata.NextLink` URL-адрес для запроса следующей страницы записей вызова. Последняя страница в диапазоне дат не имеет значения `@odata.NextLink` . Дополнительные сведения см в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging).

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.pstnCallLogRow)"
}
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.pstnCallLogRow)",
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
            "inventoryType": "Subscriber"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>См. также

* [Отчет об использовании Microsoft Teams PSTN](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [Отчет о прямой маршрутизации в Microsoft Graph](callrecords-callrecord-getdirectroutingcalls.md)
