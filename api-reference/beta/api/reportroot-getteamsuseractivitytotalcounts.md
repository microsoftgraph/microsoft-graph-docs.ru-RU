---
title: 'reportRoot: getTeamsUserActivityTotalCounts'
description: Получение количества действий Microsoft Teams по типам. Действия выполняются Microsoft Teams лицензированными или не лицензированным пользователями.
ms.localizationpriority: medium
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f0e8aed9e90d3755d9c856b6098aea66af098040
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704210"
---
# <a name="reportroot-getteamsuseractivitytotalcounts"></a>reportRoot: getTeamsUserActivityTotalCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение количества действий Microsoft Teams по типам. Действия выполняются Microsoft Teams лицензированными или не лицензированным пользователями.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

>**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalCounts(period='D7')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика. Тип выходных данных по умолчанию — text/csv. Однако если вы хотите указать тип выходных данных, можно использовать параметр запроса OData `$format` , для которого задано значение text/csv или application/json.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="response"></a>Отклик

### <a name="csv"></a>CSV

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- "Report Refresh Date" (Дата обновления отчета);
- Report Date (Дата отчета);
- Team Chat Messages (Сообщения в чатах групп);
- Отправка сообщений
- Ответные сообщения
- Private Chat Messages (Сообщения в приватных чатах);
- Calls (Звонки);
- Meetings (Собрания);
- Длительность звука
- Длительность видео
- Длительность демонстрации экрана
- Упорядоченные собрания
- Участие в собраниях
- Report Period (Отчетный период).

### <a name="json"></a>JSON

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект JSON в тексте отклика.

## <a name="example"></a>Пример

### <a name="csv"></a>CSV

Ниже приведен пример вывода CSV-файла.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Report Date,Team Chat Messages,Post Messages,Reply Messages,Private Chat Messages,Calls,Meetings,Audio Duration,Video Duration,Screen Share Duration,Meetings Organized,Meetings Attended,Report Period
```

### <a name="json"></a>JSON

Ниже приведен пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=application/json
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
Content-Length: 475

{
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "postMessages": 3,
      "replyMessages": 1,
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
      "audioDuration": 00:00:00,
      "videoDuration": 00:00:00,
      "screenShareDuration": 00:00:00,
      "meetingsOrganized": 0,
      "meetingsAttended": 0,
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
