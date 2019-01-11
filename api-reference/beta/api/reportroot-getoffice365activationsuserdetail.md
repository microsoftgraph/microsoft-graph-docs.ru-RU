---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Получите сведения о пользователях, которые активировали Office 365.
localization_priority: Normal
ms.openlocfilehash: 686a27f0942f89a9d173544d565c2562622c6e05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835282"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a>reportRoot: getOffice365ActivationsUserDetail

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получите сведения о пользователях, которые активировали Office 365.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

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
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a>Параметры запроса

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа. Выходной тип по умолчанию — текст и csv. Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="response"></a>Ответ

### <a name="csv"></a>CSV

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- "Report Refresh Date" (Дата обновления отчета);
- "User Principal Name" (Имя участника-пользователя);
- Display Name (отображаемое имя)
- Product Type (тип продукта)
- Last Activated Date (дата последней активации)
- Windows
- Mac
- Windows 10 Mobile
- iOS
- Android
- Активированные на совместно используемый компьютер

### <a name="json"></a>JSON

Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** в теле ответа.

Размер страницы по умолчанию для этого запроса — 200 элементов.

## <a name="example"></a>Пример

### <a name="csv"></a>CSV

Ниже приведен пример выводит CSV.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a>Ответ

Ниже приведен пример ответа.

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

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```

### <a name="json"></a>JSON

Ниже приведен пример, в котором возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a>Ответ

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "userActivationCounts": [
        {
          "productType": "Project Client", 
          "lastActivatedDate": "2017-08-20", 
          "windows": 5, 
          "mac": 0, 
          "windows10Mobile": 0, 
          "ios": 0, 
          "android": 2,
          "activatedOnSharedComputer": true
        }
      ]
    }
  ]
}
```
