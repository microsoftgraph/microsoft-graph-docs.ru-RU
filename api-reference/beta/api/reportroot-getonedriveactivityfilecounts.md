---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: d72a4a93fcfb9ba12d643e794d47f49239b619c6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983694"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a>reportRoot: getOneDriveActivityFileCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365: действия в OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. Обязательный. |

Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика. Тип выходных данных по умолчанию — text/csv. Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.

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
- "Viewed Or Edited" (Просмотрены или изменены);
- "Synced" (Синхронизированы);
- "Shared Internally" (К чему предоставлен доступ внутренним пользователям);
- "Shared Externally" (К чему предоставлен доступ внешним пользователям);
- "Report Date" (Дата отчета);
- Report Period (отчетный период)

### <a name="json"></a>JSON

В случае успеха этот метод возвращает код отклика и объект `200 OK` **[siteActivitySummary](../resources/siteactivitysummary.md)** в тексте отклика.

## <a name="example"></a>Пример

### <a name="csv"></a>CSV

Ниже приводится пример вывода CSV-данных.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a>JSON

Ниже приводится пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
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


