---
title: Список "Использованные"
description: Вычислите и перечислите документы, которые пользователь просматривал или изменил.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: aa18bac40b4fe7cc7b509e2948c3134ccaa77386
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001441"
---
# <a name="list-used"></a>Список "Использованные"

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вычислите и перечислите документы, которые пользователь просматривал или изменил. 

Для вошедшего пользователя:
- Этот метод включает документы, измененные пользователем; см. [Пример 1](#example-1-return-documents-that-user-has-modified). 
- Использование `$orderby` параметра запроса в свойстве **свойство lastaccesseddatetime** Возвращает самые последние просмотренные документы, которые пользователь мог или не изменил; см. [Пример 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).

Для других пользователей этот метод включает только документы, измененные пользователем.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

- Получение списка документов, измененных пользователем, вошедших в систему:
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /me/insights/used
  ```

- Получение списка документов, измененных указанным пользователем.
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  >**Примечание**. Запрос документов, **использованных** другим пользователем, возвращает результаты, отсортированные по **lastModifiedDateTime**. Затем для **свойство lastaccesseddatetime** устанавливается значение **lastModifiedDateTime**.


- Разверните ресурс, на который ссылается **использованная** аналитика:
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a>Необязательные параметры запроса
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика:

- Используйте `$filter` параметр запроса для фильтрации используемых элементов. Например, на основе **типа**:

  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- Используется `$filter` для фильтрации используемых элементов на основе  **контаинертипе**:
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).

- Используйте `$orderBy` параметр запроса, чтобы отсортировать документы, которые были просмотрены или изменены _пользователем, вошедшего_в систему, на основе свойства **свойство lastaccesseddatetime** :
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  >**Примечание**. Используйте этот параметр запроса _только для вошедшего пользователя_. Этот API нельзя использовать для получения документов, которые можно просматривать или изменять другим пользователем. См. [Пример 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).


## <a name="request-headers"></a>Заголовки запросов
| Заголовок       |  Значение|
|:-------------|:------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Accept  | application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [использованных](../resources/insights-used.md) элементов в теле отклика.

Если сведения об элементе целевого пользователя отключены, этот метод возвращает результат `403 Forbidden` и следующую ошибку:
<!-- { "blockType": "ignored" } -->

```
{
  "error": {
    "code": "ItemInsightsDisabled",
    "message": " The access to the requested resource is denied because item insights are disabled.",
    "innerError": {
      "requestId": "request-id",
      "date": "date-time"
    }
  }
}
```
Дополнительные сведения см. в статье [Настройка конфиденциальности для аналитики](/graph/insights-customize-item-insights-privacy.md). 

## <a name="example"></a>Пример

### <a name="example-1-return-documents-that-user-has-modified"></a>Пример 1: возврат документов, измененных пользователем

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "Abk3ZeZmlghMhUVKP9mygDoPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5k5RvS1T4tPmZSWjFY1PFu5N2XmZpYITIVFSj_ZsoA6BQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:38Z",
                "lastModifiedDateTime": "2019-05-25T07:12:37Z"
            },
            "resourceVisualization": {
                "title": "Org Chart",
                "type": "Visio",
                "mediaType": "application/vnd.visio",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3/thumbnails/0/small/thumbnailContent",
                "previewText": "Page-1",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/Retail/Shared Documents/NC460 Sales",
                "containerDisplayName": "Retail",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Retail/_layouts/15/Doc.aspx?sourcedoc=%7BF4463999-4FB5-4F8B-9994-968C56353C5B%7D&file=Org%20Chart.vsdx&action=default&DefaultItemOpen=1",
                "id": "drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5T7emOJwqlCit_j9Q5CpWSlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:26Z",
                "lastModifiedDateTime": "2019-05-25T07:12:26Z"
            },
            "resourceVisualization": {
                "title": "USA Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Audio Car Audio Audio - Car Audio 4910000 4664500 245500 3928000 4320800 -736500 Audi",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B637AFB94-C289-42A9-8ADF-E3F50E42A564%7D&file=USA%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INAy6LlBcXfAJCmOiEWgBJjh-lSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:11:49Z",
                "lastModifiedDateTime": "2019-05-25T07:11:48Z"
            },
            "resourceVisualization": {
                "title": "UK Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Electronics Wearable Technology Electronics - Wearable Technology 2226000 2114700 111",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B17948B2E-7C17-4202-98E8-845A00498E1F%7D&file=UK%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a>Пример 2: возврат последних просмотренных документов, которые могут быть не изменены пользователем, вошедшего в систему 

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "AWTmrUBYzTxMsvtILkUktIaN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABk5q1AWM08TLL7SC5FJLSGBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Executive Corner",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!ZOatQFjNPEyy-0guRSS0ho36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01NTE4NPQAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Executive Corner",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Exec",
                "id": "sites/m365x887078.sharepoint.com,40ade664-cd58-4c3c-b2fb-482e4524b486,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AahdFRA14_FMrGLq9V4WmyiN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACoXRUQNePxTKxi6vVeFpsoBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Contoso Landings",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!qF0VEDXj8UysYur1XhabKI36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01UHO6LBAAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Contoso Landings",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/ContosoLandings",
                "id": "sites/m365x887078.sharepoint.com,10155da8-e335-4cf1-ac62-eaf55e169b28,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IztQAKAS6acR7HFoIKDqOPE6bjkeoHWtEu7LoUIsZkHSkzLaA_67htEozMGRwifyaqlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:54Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Media Preview Packages",
                "type": "Web",
                "mediaType": "text/html",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jO1AAoBLppxHscWggoOo48TpuOR6gda0S7suhQixmQdK/items/01RGQ6XKCMZNUA76XODNCKGMYGI4EJ7SNK/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Forms/ByAuthor.aspx",
                "containerDisplayName": "Campaigns - Events"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Media-Preview-Packages.aspx"
            }
        }
    ]
}
```


