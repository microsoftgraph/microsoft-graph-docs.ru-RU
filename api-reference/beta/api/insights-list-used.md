---
title: Список "Использованные"
description: Вычислите и перечислите документы, которые пользователь просматривал или изменил.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 4b9eacacaf808330efa5b9d41face09e3cbbfd7d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964620"
---
# <a name="list-used"></a><span data-ttu-id="022f1-103">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="022f1-103">List used</span></span>

<span data-ttu-id="022f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="022f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="022f1-105">Вычислите и перечислите документы, которые пользователь просматривал или изменил.</span><span class="sxs-lookup"><span data-stu-id="022f1-105">Calculate and list the documents that a user has viewed or modified.</span></span> 

<span data-ttu-id="022f1-106">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="022f1-106">For the signed-in user:</span></span>
- <span data-ttu-id="022f1-107">Этот метод включает документы, измененные пользователем; см. [Пример 1](#example-1-return-documents-that-user-has-modified).</span><span class="sxs-lookup"><span data-stu-id="022f1-107">This method includes documents that the user has modified; see [example 1](#example-1-return-documents-that-user-has-modified).</span></span> 
- <span data-ttu-id="022f1-108">Использование `$orderby` параметра запроса в свойстве **свойство lastaccesseddatetime** Возвращает самые последние просмотренные документы, которые пользователь мог или не изменил; см. [Пример 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="022f1-108">Using an `$orderby` query parameter on the **lastAccessedDateTime** property returns the most recently viewed documents that the user might or might not have modified; see [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>

<span data-ttu-id="022f1-109">Для других пользователей этот метод включает только документы, измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="022f1-109">For other users, this method includes only documents that the user has modified.</span></span>


## <a name="permissions"></a><span data-ttu-id="022f1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="022f1-110">Permissions</span></span>
<span data-ttu-id="022f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="022f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="022f1-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="022f1-113">Permission type</span></span>      | <span data-ttu-id="022f1-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="022f1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="022f1-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="022f1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="022f1-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="022f1-116">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="022f1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="022f1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="022f1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="022f1-118">Not supported.</span></span>    |
|<span data-ttu-id="022f1-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="022f1-119">Application</span></span> | <span data-ttu-id="022f1-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="022f1-120">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="022f1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="022f1-121">HTTP request</span></span>

- <span data-ttu-id="022f1-122">Получение списка документов, измененных пользователем, вошедших в систему:</span><span class="sxs-lookup"><span data-stu-id="022f1-122">Get a list of documents that the signed-in user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /me/insights/used
  ```

- <span data-ttu-id="022f1-123">Получение списка документов, измененных указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="022f1-123">Get a list of documents that the specified user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  ><span data-ttu-id="022f1-124">**Примечание**. Запрос документов, **использованных** другим пользователем, возвращает результаты, отсортированные по **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="022f1-124">**Note** : Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="022f1-125">Затем для **свойство lastaccesseddatetime** устанавливается значение **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="022f1-125">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>


- <span data-ttu-id="022f1-126">Разверните ресурс, на который ссылается **использованная** аналитика:</span><span class="sxs-lookup"><span data-stu-id="022f1-126">Expand the resource referenced by a **used** insight:</span></span>
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a><span data-ttu-id="022f1-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="022f1-127">Optional query parameters</span></span>
<span data-ttu-id="022f1-128">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика:</span><span class="sxs-lookup"><span data-stu-id="022f1-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- <span data-ttu-id="022f1-129">Используйте `$filter` параметр запроса для фильтрации используемых элементов.</span><span class="sxs-lookup"><span data-stu-id="022f1-129">Use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="022f1-130">Например, на основе **типа** :</span><span class="sxs-lookup"><span data-stu-id="022f1-130">For example, based on **type** :</span></span>

  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- <span data-ttu-id="022f1-131">Используется `$filter` для фильтрации используемых элементов на основе  **контаинертипе** :</span><span class="sxs-lookup"><span data-stu-id="022f1-131">Use `$filter` to filter used items based on  **containerType** :</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  <span data-ttu-id="022f1-132">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="022f1-132">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

- <span data-ttu-id="022f1-133">Используйте `$orderBy` параметр запроса, чтобы отсортировать документы, которые были просмотрены или изменены _пользователем, вошедшего_ в систему, на основе свойства **свойство lastaccesseddatetime** :</span><span class="sxs-lookup"><span data-stu-id="022f1-133">Use the `$orderBy` query parameter to sort documents last viewed or modified _by the signed-in user_ , based on the **lastAccessedDateTime** property:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  ><span data-ttu-id="022f1-134">**Примечание**. Используйте этот параметр запроса _только для вошедшего пользователя_.</span><span class="sxs-lookup"><span data-stu-id="022f1-134">**Note** : Use this query option _only for the signed-in user_.</span></span> <span data-ttu-id="022f1-135">Этот API нельзя использовать для получения документов, которые можно просматривать или изменять другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="022f1-135">You cannot use this API to get documents viewed or modified by another user.</span></span> <span data-ttu-id="022f1-136">См. [Пример 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="022f1-136">See [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>


## <a name="request-headers"></a><span data-ttu-id="022f1-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="022f1-137">Request headers</span></span>
| <span data-ttu-id="022f1-138">Заголовок</span><span class="sxs-lookup"><span data-stu-id="022f1-138">Header</span></span>       |  <span data-ttu-id="022f1-139">Значение</span><span class="sxs-lookup"><span data-stu-id="022f1-139">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="022f1-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="022f1-140">Authorization</span></span>  | <span data-ttu-id="022f1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="022f1-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="022f1-143">Accept</span><span class="sxs-lookup"><span data-stu-id="022f1-143">Accept</span></span>  | <span data-ttu-id="022f1-144">application/json</span><span class="sxs-lookup"><span data-stu-id="022f1-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="022f1-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="022f1-145">Request body</span></span>
<span data-ttu-id="022f1-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="022f1-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="022f1-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="022f1-147">Response</span></span>

<span data-ttu-id="022f1-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [использованных](../resources/insights-used.md) элементов в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="022f1-148">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>

<span data-ttu-id="022f1-149">Если сведения об элементе целевого пользователя отключены, этот метод возвращает результат `403 Forbidden` и следующую ошибку:</span><span class="sxs-lookup"><span data-stu-id="022f1-149">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
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
<span data-ttu-id="022f1-150">Дополнительные сведения см. в статье [Настройка конфиденциальности для аналитики](/graph/insights-customize-item-insights-privacy.md).</span><span class="sxs-lookup"><span data-stu-id="022f1-150">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span> 

## <a name="example"></a><span data-ttu-id="022f1-151">Пример</span><span class="sxs-lookup"><span data-stu-id="022f1-151">Example</span></span>

### <a name="example-1-return-documents-that-user-has-modified"></a><span data-ttu-id="022f1-152">Пример 1: возврат документов, измененных пользователем</span><span class="sxs-lookup"><span data-stu-id="022f1-152">Example 1: Return documents that user has modified</span></span>

#### <a name="request"></a><span data-ttu-id="022f1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="022f1-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="022f1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="022f1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used
```
# <a name="c"></a>[<span data-ttu-id="022f1-155">C#</span><span class="sxs-lookup"><span data-stu-id="022f1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="022f1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="022f1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="022f1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="022f1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="022f1-158">Java</span><span class="sxs-lookup"><span data-stu-id="022f1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifieddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="022f1-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="022f1-159">Response</span></span>

><span data-ttu-id="022f1-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="022f1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
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

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a><span data-ttu-id="022f1-162">Пример 2: возврат последних просмотренных документов, которые могут быть не изменены пользователем, вошедшего в систему</span><span class="sxs-lookup"><span data-stu-id="022f1-162">Example 2: Return the most recently viewed documents that the signed-in user might or might not have modified</span></span> 

#### <a name="request"></a><span data-ttu-id="022f1-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="022f1-163">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="022f1-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="022f1-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[<span data-ttu-id="022f1-165">C#</span><span class="sxs-lookup"><span data-stu-id="022f1-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="022f1-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="022f1-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="022f1-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="022f1-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="022f1-168">Java</span><span class="sxs-lookup"><span data-stu-id="022f1-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifiedandvieweddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="022f1-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="022f1-169">Response</span></span>
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


