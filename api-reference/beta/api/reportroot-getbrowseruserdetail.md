---
title: 'reportRoot: getBrowserUserDetail'
description: Получите отчет, который предоставляет браузеры (Microsoft Edge, устаревшая версия Microsoft Edge и Internet Explorer), используемые пользователями при доступе к Microsoft 365 службам в течение определенного периода.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ea0d22e55ee707f3cb7a3180a2d35572c52f80c0
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589854"
---
# <a name="reportroot-getbrowseruserdetail"></a>reportRoot: getBrowserUserDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите отчет, который предоставляет браузеры (Microsoft Edge, устаревшая версия Microsoft Edge и Internet Explorer), используемые пользователями при доступе к Microsoft 365 службам в течение определенного периода.

> **Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 Отчеты в центре администрирования — использование браузера Майкрософт](/microsoft-365/admin/activity-reports/browser-usage-report).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                            |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Reports.Read.All                            |

> **Примечание:** Для делегирования разрешений, позволяющих приложениям читать отчеты об использовании служб от имени пользователя, администратор клиента должен присвоить пользователю соответствующую Azure Active Directory роль администратора. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getBrowserUserDetail(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.

| Параметр | Тип   | Описание                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value} : `D7`, , `D30`и `D90``D180`. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа. Тип вывода по умолчанию `text/csv`. Однако если требуется указать тип вывода, можно использовать параметр запроса OData `$format` , чтобы задать выход по умолчанию `text/csv` или `application/json`.

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
- "User Principal Name" (Имя участника-пользователя);
- Report Period (Отчетный период).
- Microsoft Edge
- Edge Legacy
- Internet Explorer

### <a name="json"></a>JSON

В случае успешной работы этот метод возвращает код `200 OK` отклика и объект JSON в тексте ответа.

Размер страницы по умолчанию для этого запроса составляет 200 элементов.

## <a name="examples"></a>Примеры

### <a name="example-1-csv-output"></a>Пример 1. Выход CSV

Ниже приводится пример, который выводит CSV.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getbrowseruserdetail_csv"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getBrowserUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.


<!-- { "blockType": "response" } -->
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

Report Refresh Date, User Principal Name, Report Period, Edge, Edge Legacy, Internet Explorer
```

### <a name="example-2-json-output"></a>Пример 2. Вывод JSON

Ниже приводится пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getbrowseruserdetail_json"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getBrowserUserDetail(period='D7')?$format=application/json
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
Content-Length: 304

{
  "@odata.nextLink": "https://graph.microsoft.com/beta/reports/getBrowserUserDetail(period='D7')?$format=application/json&$skiptoken=D07uj",
   "value":[
      {
         "reportRefreshDate":"2021-04-17",
         "userPrincipalName": "admin@contoso.com",
         "details":[
            {
               "reportPeriod":7,
               "edge":true,
               "edgeLegacy":true,
               "ie":false
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
