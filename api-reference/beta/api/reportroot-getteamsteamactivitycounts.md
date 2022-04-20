---
title: 'reportRoot: getTeamsTeamActivityCounts'
description: Получение количества командных действий в Microsoft Teams. Типы действий связаны с собраниями и сообщениями.
ms.localizationpriority: medium
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0735c07c4d0799e7510915f00eafbc393782f86d
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917927"
---
# <a name="reportroot-getteamsteamactivitycounts"></a>reportRoot: getTeamsTeamActivityCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение количества командных действий в Microsoft Teams. Типы действий связаны с собраниями и сообщениями.

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
GET /reports/getTeamsTeamActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите следующие параметры с допустимым значением.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения для {period_value}: `D7`, `D30`, и `D90``D180`. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный. |
| date      | Date   | Указывает дату, в течение которой вы хотите просмотреть сведения о действиях в командах. Значение {date_value} указывается в формате ГГГГ-ММ-ДД. Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона. |

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
- Report Period (Отчетный период).
- Report Date (дата отчета)
- Активные пользователи
- Активные каналы
- Гости
- Реакции
- Упорядоченные собрания
- Отправка сообщений
- Сообщения канала
- Активные общие каналы
- Активные внешние пользователи
- Ответные сообщения
- Срочные сообщения
- Упоминания

### <a name="json"></a>JSON

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект JSON в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-csv-output"></a>Пример 1. Выходные данные CSV

Ниже приведен пример вывода CSV-файла.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsteamactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Report Period,Report Date,Active Users,Active Channels,Guests,Reactions,Meetings Organized,Post Messages,Channel Messages,Active Shared Channels,Active External Users,Reply Messages,Urgent Messages,Mentions
```

### <a name="example-2-json-output"></a>Пример 2. Выходные данные JSON

Ниже приведен пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsteamactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityCounts(period='D7')?$format=application/json
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
Content-Length: 641

{
  "@odata.context": "https://graph.microsoft.com/beta/reports/getTeamsTeamActivityCounts(period='D7')?$format=application/json&$skiptoken=D07uj", 
  "value": [
    {
      "reportRefreshDate": "2021-09-01", 
      "reportPeriod":7,
      "userCounts": [
        {
          "reportDate": "2021-09-01", 
          "activeUsers": 26, 
          "activeChannels": 17, 
          "guests": 4, 
          "reactions": 36, 
          "meetingsOrganized": 0,
          "postMessages": 83,
          "channelMessages": 101,
          "activeSharedChannels": 1,
          "activeExternalUsers": 2,
          "replyMessages":10,
          "urgentMessages":8,
          "mentions":1
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
