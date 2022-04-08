---
title: 'reportRoot: getTeamsUserActivityTotalDistributionCounts'
description: Получение количества действий Microsoft Teams за выбранный период. Типы действий — это сообщения в чате группы, личные сообщения чата, звонки, собрания, организованные собрания, собрания, длительность звука, длительность видео, продолжительность демонстрации экрана, отправка сообщений и ответных сообщений.
ms.localizationpriority: medium
ms.prod: reports
author: zhiliqiao
doc_type: apiPageType
ms.openlocfilehash: bfd2c37c542392022e0347089f0a1b4382265842
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704488"
---
# <a name="reportroot-getteamsuseractivitytotaldistributioncounts"></a>reportRoot: getTeamsUserActivityTotalDistributionCounts
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение количества действий Microsoft Teams за выбранный период. Типы действий — это сообщения в чате группы, личные сообщения чата, звонки, собрания, организованные собрания, собрания, длительность звука, длительность видео, продолжительность демонстрации экрана, отправка сообщений и ответных сообщений.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

> **Примечание**. Для делегированных разрешений, позволяющих приложениям считывать отчеты об использовании служб от имени пользователя, администратор клиента должен назначить пользователю соответствующую роль Azure Active Directory администратора. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalDistributionCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения для {period_value}: `D7`, `D30`, и `D90``D180`. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный.|

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа. Тип выходных данных по умолчанию — `text/csv`.. Однако если вы хотите указать тип выходных данных, можно использовать параметр запроса OData `$format` для задания выходных данных по умолчанию `application/json`или `text/csv` .

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

### <a name="csv"></a>CSV

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- Report Refresh Date (Дата обновления отчета);
- Team Chat Messages (Сообщения в чатах групп);
- Private Chat Messages (Сообщения в приватных чатах);
- Calls (Звонки);
- Meetings (Собрания);
- Упорядоченные собрания
- Участие в собраниях
- Длительность звука
- Длительность видео
- Длительность демонстрации экрана
- Отправка сообщений
- Ответные сообщения
- Report Period (Отчетный период).

### <a name="json"></a>JSON

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект JSON в тексте отклика.

Размер страницы по умолчанию для этого запроса — 2000 элементов.

## <a name="examples"></a>Примеры

### <a name="example-1-csv-output"></a>Пример 1. Выходные данные CSV

Ниже приведен пример вывода CSV-файла.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalDistributionCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Meetings Organized,Meetings Attended,Audio Duration,Video Duration,Screen Share Duration,Post Messages,Reply Messages,Report Period
```

### <a name="example-2-json-output"></a>Пример 2. Выходные данные JSON

Ниже приведен пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalDistributionCounts(period='D7')?$format=application/json
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
Content-Length: 661

{
  "@odata.context": "https://graph.microsoft.com/beta/getTeamsUserActivityTotalDistributionCounts(period='D7')?$format=application/json&$skiptoken=D07uj", 
  "value": [
      "reportRefreshDate": "2021-09-01", 
      "userCounts"
        {
          "reportPeriod":7,
          "teamChatMessages": 26, 
          "privateChatMessages": 17, 
          "calls": 4, 
          "meetings": 0, 
          "audioDuration": 00:00:00,
          "videoDuration": 00:00:00,
          "screenShareDuration": 00:00:00,
          "meetingsOrganized": 0,
          "meetingsAttended": 0,
          "postMessages": 1,
          "replyMessages": 1
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


