---
title: 'reportRoot: getTeamsTeamActivityDetail'
description: Получение сведений о Microsoft Teams действий по командам. Эти числа включают действия как для лицензированных, так и для пользователей без лицензии.
ms.localizationpriority: medium
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7acd09947d4c37eb803f14cdc0cff508fac60172
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917948"
---
# <a name="reportroot-getteamsteamactivitydetail"></a>reportRoot: getTeamsTeamActivityDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение сведений о Microsoft Teams действий по командам. Эти числа включают действия как для лицензированных, так и для пользователей без лицензии.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

> **Примечание:** Чтобы делегированные разрешения разрешать приложениям считывать отчеты об использовании служб от имени пользователя, администратор клиента должен назначить пользователю соответствующую роль Azure Active Directory администратора. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsTeamActivityDetail(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите следующие параметры с допустимым значением.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения для {period_value}: `D7`, `D30`, и `D90``D180`. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный. |
| date      | Date   | Указывает дату, в течение которой вы хотите просмотреть сведения о действиях в одной или нескольких командах. Значение {date_value} указывается в формате ГГГГ-ММ-ДД. Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона. |

> **Примечание:** Необходимо задать точку **или** дату **в** URL-адресе запроса.

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика. Тип выходных данных по умолчанию — `text/csv`.. Однако если вы хотите указать тип выходных данных, можно использовать параметр запроса OData `$format` для задания выходных данных по умолчанию `application/json`или `text/csv` .

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="response"></a>Отклик

### <a name="csv"></a>CSV

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- Report Refresh Date (Дата обновления отчета);
- Имя группы
- Идентификатор команды
- Тип команды
- Last Activity Date (Дата последнего действия);
- Report Period (Отчетный период).
- Активные пользователи
- Активные каналы
- Гости
- Реакции
- Упорядоченные собрания
- Отправка сообщений
- Ответные сообщения
- Сообщения канала
- Срочные сообщения
- Упоминания
- Активные общие каналы
- Активные внешние пользователи

### <a name="json"></a>JSON

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект JSON в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-csv-output"></a>Пример 1. Выходные данные CSV

Ниже приведен пример вывода CSV-файла.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDetail(period='D7')?$format=text/csv
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

Report Refresh Date,Team Name,Team Id,Team Type,Last Activity Date,Report Period,Active Users,Active Channels,Guests,Reactions,Meetings Organized,Post Messages,Reply Messages,Channel Messages,Urgent Messages,Mentions,Active Shared Channels,Active External Users
```

### <a name="example-2-json-output"></a>Пример 2. Выходные данные JSON

Ниже приведен пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDetail(period='D7')?$format=application/json
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
Content-Length: 876

{
  "@odata.context": "https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDetail(period='D7')?$format=application/json&$skiptoken=D07uj", 
  "value": [
    {
      "reportRefreshDate": "2021-09-01", 
      "teamName": "sampleTeam",
      "teamId": "a063d832-ae9a-467d-8cb4-17c073260890",
      "teamType": "Private",
      "lastActivityDate": "2021-09-01",
      "details": [
        {
          "reportPeriod":7,
          "activeUsers": 26, 
          "activeChannels": 17, 
          "guests": 4, 
          "reactions": 36, 
          "meetingsOrganized": 0,
          "postMessages": 0,
          "replyMessages": 0,
          "channelMessages": 0,
          "urgentMessages": 0,
          "mentions": 0,
          "activeSharedChannels": "6",
          "activeExternalUsers": "8"
        }
      ]
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
