---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ebcc0285558099d46708c70feec1252b3f2e6494
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265179"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a>reportRoot: getSkypeForBusinessParticipantActivityUserCounts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия участников конференций Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде. Обязательный. |

Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика. Тип выходных данных по умолчанию — Text/CSV. Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.

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
- "Report Date" (Дата отчета);
- "Report Period" (Отчетный период);
- "IM" (Обмен мгновенными сообщениями);
- "Audio/Video" (Аудио и видео);
- "App Sharing" (Общий доступ к приложениям);
- "Web" (Интернет);
- "Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба).

### <a name="json"></a>JSON

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспартиЦипантактивитюсеркаунтс](../resources/skypeforbusinessparticipantactivityusercounts.md)** в тексте отклика.

## <a name="example"></a>Пример

### <a name="csv"></a>CSV

Ниже приведен пример выходных данных CSV.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a>Образец кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a>JSON

Ниже приведен пример, в котором возвращается JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
