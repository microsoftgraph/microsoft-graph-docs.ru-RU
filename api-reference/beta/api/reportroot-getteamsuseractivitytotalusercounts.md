---
title: 'reportRoot: getTeamsUserActivityTotalUserCounts'
description: Получите число пользователей, Microsoft Teams лицензированных или не лицензированных пользователей по типу действия. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.
ms.localizationpriority: medium
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2406a62d4b239f7e4d65bbb4b51b0dd26054aab9
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044759"
---
# <a name="reportroot-getteamsuseractivitytotalusercounts"></a>reportRoot: getTeamsUserActivityTotalUserCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите число пользователей, Microsoft Teams лицензированных или не лицензированных пользователей по типу действия. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

> **Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalUserCounts(period='D7')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика. Тип вывода по умолчанию — текст/csv. Однако если требуется указать тип вывода, можно использовать параметр запроса OData, заданный для `$format` text/csv или application/json.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

### <a name="csv"></a>CSV

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- "Report Refresh Date" (Дата обновления отчета);
- Report Date (Дата отчета);
- Team Chat Messages (Сообщения в чатах групп);
- Private Chat Messages (Сообщения в приватных чатах);
- Calls (Звонки);
- Meetings (Собрания);
- Other Actions (Другие действия);
- Report Period (Отчетный период).

### <a name="json"></a>JSON

В случае успешной работы этот метод возвращает код отклика и `200 OK` объект JSON в тексте ответа.

## <a name="example"></a>Пример

### <a name="csv"></a>CSV

Ниже приводится пример, который выводит CSV.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```

### <a name="json"></a>JSON

Ниже приводится пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
