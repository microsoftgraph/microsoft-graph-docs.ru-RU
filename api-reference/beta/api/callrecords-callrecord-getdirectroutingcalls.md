---
title: 'callRecord: getDirectRoutingCalls'
description: Получите журнал прямых вызовов маршрутизов.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 85d6b54f0cde797757f5e8711c1ae058a668dd95
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786917"
---
# <a name="callrecord-getdirectroutingcalls"></a>callRecord: getDirectRoutingCalls

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите журнал прямых маршрутизировок в качестве коллекции записей [directRoutingLogRow.](../resources/callrecords-directroutinglogrow.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Application                            | CallRecord-PstnCalls.Read.All, CallRecords.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getDirectRoutingCalls
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.
В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.

|Параметр|Тип|Описание|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|Начало диапазона времени для запроса. UTC включительно.<br/>Диапазон времени зависит от времени начала вызова.|
|toDateTime|DateTimeOffset|Конец диапазона времени для запроса. UTC включительно.|

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код отклика и коллекцию записей `200 OK` [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) в тексте ответа.
  
Если в диапазоне дат более 1000 записей, тело также включает URL-адрес для запроса следующей страницы записей `@odata.NextLink` вызовов. Последняя страница в диапазоне дат не имеет `@odata.NextLink` . Дополнительные сведения см. [в Graph microsoft Graph в приложении.](/graph/paging)

## <a name="example"></a>Пример

В следующем примере показано, как получить коллекцию записей для прямых вызовов маршрутов, которые произошли в указанном диапазоне дат. Ответ включает в себя список записей в этом первом ответе и получения записей за пределами первых `"@odata.count": 1000` `@odata.NextLink` 1000. Для читаемости в ответе показана только коллекция из 1 записи. Предположим, что в этом диапазоне дат более 1000 вызовов.

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "isCollection": true
} 
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.directRoutingLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9e8bba57-dc14-533a-a7dd-f0da6575eed1",
            "correlationId": "c98e1515-a937-4b81-b8a8-3992afde64e0",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:25.105Z",
            "inviteDateTime": "2019-11-01T00:00:21.949Z",
            "failureDateTime": "0001-01-01T00:00:00Z",
            "endDateTime": "2019-11-01T00:00:30.105Z",
            "duration": 5,
            "callType": "ByotIn",
            "successfulCall": true,
            "callerNumber": "+12345678***",
            "calleeNumber": "+01234567***",
            "mediaPathLocation": "USWE",
            "signalingLocation": "EUNO",
            "finalSipCode": 0,
            "callEndSubReason": 540000,
            "finalSipCodePhrase": "BYE",
            "trunkFullyQualifiedDomainName": "tll-audiocodes01.adatum.biz",
            "mediaBypassEnabled": false
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>См. также

* [Microsoft Teams отчет об использовании маршрутов](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) в центре Microsoft Teams администрирования.
* [Панель мониторинга состояния здоровья для прямой маршрутивки](/MicrosoftTeams/direct-routing-health-dashboard) в центре администрирования Microsoft Teams области.
* [Отчет о вызове PSTN в Microsoft Graph](callrecords-callrecord-getpstncalls.md).