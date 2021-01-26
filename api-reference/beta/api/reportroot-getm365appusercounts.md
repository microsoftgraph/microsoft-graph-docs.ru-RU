---
title: 'reportRoot: getM365AppUserCounts'
description: Получите отчет, который обеспечивает тенденцию числа активных пользователей для каждого приложения — Outlook, Word, Excel, PowerPoint, OneNote и Teams — в вашей организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 3c415e973e2e0e84edb306d9e64a024f91b1a905
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981356"
---
# <a name="reportroot-getm365appusercounts"></a>reportRoot: getM365AppUserCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите отчет, который обеспечивает тенденцию числа активных пользователей для каждого приложения — Outlook, Word, Excel, PowerPoint, OneNote и Teams — в вашей организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании приложений Microsoft 365.](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                            |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Reports.Read.All                            |

> **Примечание.** Чтобы делегировать разрешения, позволяющие приложениям читать отчеты об использовании служб от имени пользователя, администратор клиента должен на назначенную пользователю роль ограниченного администратора Azure AD. Подробные сведения [см. в авторизации для API для чтения отчетов об использовании Microsoft 365.](/graph/reportroot-authorization)

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.

| Параметр | Тип   | Описание                                                                                                                                                                                                                                                       |
| :-------- | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения для {period_value}: `D7` , `D30` , и `D90` `D180` . Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика. Тип выходных данных по умолчанию — text/csv. Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData, чтобы задать для выходных данных по умолчанию значение `$format` text/csv или application/json.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и `200 OK` объект [отчета](../resources/intune-shared-report.md) в тексте отклика. Данные отчета содержатся в свойстве **контента** объекта **отчета.**

### <a name="csv"></a>CSV

В случае успешного запроса свойства **контента** возвращается ответ, который перенаправляет на URL-адрес предварительной загрузки для `302 Found` отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- Report Refresh Date (Дата обновления отчета);
- "Report Period" (Отчетный период).
- Report Date (дата отчета)
- Outlook
- Word
- Excel
- PowerPoint
- OneNote
- Teams

### <a name="json"></a>JSON

В случае успешного запроса свойства **контента** возвращается `200 OK` код отклика и объект JSON в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-csv-output"></a>Пример 1. Выходные данные CSV

Ниже приводится пример вывода CSV-данных.

#### <a name="request"></a>Запрос

Ниже приводится пример запроса на получения **свойства контента.**



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserCounts(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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

Report Refresh Date,Report Period,Report Date,Outlook,Word,Excel,PowerPoint,OneNote,Teams
```

### <a name="example-2-json-output"></a>Пример 2. Выходные данные JSON

Ниже приводится пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приводится пример запроса на получения **свойства контента.**



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserCounts(period='D7')/content?$format=application/json
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "reportPeriod": 7,
      "userCounts": [
        {
          "reportDate": "2020-06-30",
          "outlook": 1513,
          "word": 911,
          "excel": 790,
          "powerPoint": 683,
          "oneNote": 969,
          "teams": 1532
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
