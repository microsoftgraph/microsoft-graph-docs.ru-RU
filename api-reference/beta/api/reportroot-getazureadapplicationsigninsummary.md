---
title: 'reportRoot: getAzureADApplicationSignInSummary'
description: Получение свойств и связей объекта applicationSigninSummary.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 982fd527b12da40e13d48d3d9b31df8dcab34adc
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647079"
---
# <a name="reportroot-getazureadapplicationsigninsummary"></a>reportRoot: getAzureADApplicationSignInSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение [объектов applicationSigninSummary](../resources/applicationsigninsummary.md) в течение последних семи или 30 дней.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Reports.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается   |
|Для приложений | Reports.Read.All | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a>Параметры функции

| Параметр | Описание |
|:----------|:----------|
| period | (последние `D7` семь дней) или `D30` (последние 30 дней); другие значения создают ошибки. |

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` [applicationSignInSummary](../resources/applicationsigninsummary.md) в тексте ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsigninsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(applicationSignInSummary)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.applicationSignInSummary",
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "successfulSignInCount": 9,
            "failedSignInCount": 0,
            "appDisplayName": "Graph Explorer",
            "successPercentage": 100
        },
        {
            "@odata.type": "#microsoft.graph.applicationSignInSummary",
            "id": "c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
            "successfulSignInCount": 2,
            "failedSignInCount": 0,
            "appDisplayName": "Azure Portal",
            "successPercentage": 100
        },
        {
            "@odata.type": "#microsoft.graph.applicationSignInSummary",
            "id": "8c59ead7-d703-4a27-9e55-c96a0054c8d2",
            "successfulSignInCount": 1,
            "failedSignInCount": 0,
            "appDisplayName": "My Profile",
            "successPercentage": 100
        },
        {
            "@odata.type": "#microsoft.graph.applicationSignInSummary",
            "id": "89bee1f7-5e6e-4d8a-9f3d-ecd601259da7",
            "successfulSignInCount": 3,
            "failedSignInCount": 0,
            "appDisplayName": "Office365 Shell WCSS-Client",
            "successPercentage": 100
        }
    ]
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


