---
title: Список "Использованные"
description: Вычислять и перечислять документы, которые пользователь просмотрел или изменил.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: b29089bf5cfe87ad0aede192a1c89430fc51b5e6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473229"
---
# <a name="list-used"></a><span data-ttu-id="361d1-103">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="361d1-103">List used</span></span>

<span data-ttu-id="361d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="361d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="361d1-105">Вычислять и перечислять документы, которые пользователь просмотрел или изменил.</span><span class="sxs-lookup"><span data-stu-id="361d1-105">Calculate and list the documents that a user has viewed or modified.</span></span> 

<span data-ttu-id="361d1-106">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="361d1-106">For the signed-in user:</span></span>
- <span data-ttu-id="361d1-107">Этот метод включает документы, которые пользователь изменил; см. [пример 1](#example-1-return-documents-that-user-has-modified).</span><span class="sxs-lookup"><span data-stu-id="361d1-107">This method includes documents that the user has modified; see [example 1](#example-1-return-documents-that-user-has-modified).</span></span> 
- <span data-ttu-id="361d1-108">Использование параметра запроса в свойстве `$orderby` **lastAccessedDateTime** возвращает самые недавно просмотренные документы, которые пользователь мог изменить или не изменить; см. пример [2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="361d1-108">Using an `$orderby` query parameter on the **lastAccessedDateTime** property returns the most recently viewed documents that the user might or might not have modified; see [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>

<span data-ttu-id="361d1-109">Для других пользователей этот метод включает только документы, измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="361d1-109">For other users, this method includes only documents that the user has modified.</span></span>


## <a name="permissions"></a><span data-ttu-id="361d1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="361d1-110">Permissions</span></span>
<span data-ttu-id="361d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="361d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="361d1-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="361d1-113">Permission type</span></span>      | <span data-ttu-id="361d1-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="361d1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="361d1-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="361d1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="361d1-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="361d1-116">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="361d1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="361d1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="361d1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="361d1-118">Not supported.</span></span>    |
|<span data-ttu-id="361d1-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="361d1-119">Application</span></span> | <span data-ttu-id="361d1-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="361d1-120">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="361d1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="361d1-121">HTTP request</span></span>

- <span data-ttu-id="361d1-122">Получите список документов, которые изменил пользователь, вписанный в него:</span><span class="sxs-lookup"><span data-stu-id="361d1-122">Get a list of documents that the signed-in user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /me/insights/used
  ```

- <span data-ttu-id="361d1-123">Получите список документов, измененных указанным пользователем:</span><span class="sxs-lookup"><span data-stu-id="361d1-123">Get a list of documents that the specified user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  ><span data-ttu-id="361d1-124">**Примечание.** Запрос документов, используемых другим **пользователем,** возвращает результаты, отсортифицированные **lastModifiedDateTime.**</span><span class="sxs-lookup"><span data-stu-id="361d1-124">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="361d1-125">**LastAccessedDateTime** затем устанавливается **lastModifiedDateTime.**</span><span class="sxs-lookup"><span data-stu-id="361d1-125">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>


- <span data-ttu-id="361d1-126">Расширение ресурса, на который ссылается **использованная информация:**</span><span class="sxs-lookup"><span data-stu-id="361d1-126">Expand the resource referenced by a **used** insight:</span></span>
  <!-- { "blockType": "ignored" } -->
  
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a><span data-ttu-id="361d1-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="361d1-127">Optional query parameters</span></span>
<span data-ttu-id="361d1-128">Этот метод поддерживает [параметры запроса OData](/graph/query-parameters) для настройки ответа:</span><span class="sxs-lookup"><span data-stu-id="361d1-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- <span data-ttu-id="361d1-129">Используйте параметр `$filter` запроса для фильтрации используемых элементов.</span><span class="sxs-lookup"><span data-stu-id="361d1-129">Use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="361d1-130">Например, в зависимости от **типа:**</span><span class="sxs-lookup"><span data-stu-id="361d1-130">For example, based on **type**:</span></span>

  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- <span data-ttu-id="361d1-131">Использование `$filter` для фильтрации используемых элементов на основе **containerType:**</span><span class="sxs-lookup"><span data-stu-id="361d1-131">Use `$filter` to filter used items based on  **containerType**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  <span data-ttu-id="361d1-132">В [resourceVisualization](../resources/insights-resourcevisualization.md)см. доступные типы и типы контейнеров, которые можно фильтровать.</span><span class="sxs-lookup"><span data-stu-id="361d1-132">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

- <span data-ttu-id="361d1-133">Используйте параметр запроса для сортировки документов, которые последний раз просматривались или изменены пользователем, в соответствии с свойством `$orderBy` **lastAccessedDateTime:** </span><span class="sxs-lookup"><span data-stu-id="361d1-133">Use the `$orderBy` query parameter to sort documents last viewed or modified _by the signed-in user_, based on the **lastAccessedDateTime** property:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  ><span data-ttu-id="361d1-134">**Примечание.** Используйте этот параметр запроса только для _подписанного пользователя._</span><span class="sxs-lookup"><span data-stu-id="361d1-134">**Note**: Use this query option _only for the signed-in user_.</span></span> <span data-ttu-id="361d1-135">Этот API нельзя использовать для просмотра или изменения документов другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="361d1-135">You cannot use this API to get documents viewed or modified by another user.</span></span> <span data-ttu-id="361d1-136">См. [пример 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="361d1-136">See [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>


## <a name="request-headers"></a><span data-ttu-id="361d1-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="361d1-137">Request headers</span></span>
| <span data-ttu-id="361d1-138">Заголовок</span><span class="sxs-lookup"><span data-stu-id="361d1-138">Header</span></span>       |  <span data-ttu-id="361d1-139">Значение</span><span class="sxs-lookup"><span data-stu-id="361d1-139">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="361d1-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="361d1-140">Authorization</span></span>  | <span data-ttu-id="361d1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="361d1-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="361d1-143">Accept</span><span class="sxs-lookup"><span data-stu-id="361d1-143">Accept</span></span>  | <span data-ttu-id="361d1-144">application/json</span><span class="sxs-lookup"><span data-stu-id="361d1-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="361d1-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="361d1-145">Request body</span></span>
<span data-ttu-id="361d1-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="361d1-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="361d1-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="361d1-147">Response</span></span>

<span data-ttu-id="361d1-148">В случае успешного использования этот метод возвращает код ответа и список используемых элементов `200 OK` в тексте [](../resources/insights-used.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="361d1-148">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>

<span data-ttu-id="361d1-149">Если представление элементов целевого пользователя отключено, этот метод возвращается `403 Forbidden` и следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="361d1-149">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
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
<span data-ttu-id="361d1-150">Дополнительные сведения см. в статье [Настройка конфиденциальности для аналитики](/graph/insights-customize-item-insights-privacy.md).</span><span class="sxs-lookup"><span data-stu-id="361d1-150">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span> 

## <a name="example"></a><span data-ttu-id="361d1-151">Пример</span><span class="sxs-lookup"><span data-stu-id="361d1-151">Example</span></span>

### <a name="example-1-return-documents-that-user-has-modified"></a><span data-ttu-id="361d1-152">Пример 1. Возвращение документов, измененных пользователем</span><span class="sxs-lookup"><span data-stu-id="361d1-152">Example 1: Return documents that user has modified</span></span>

#### <a name="request"></a><span data-ttu-id="361d1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="361d1-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="361d1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="361d1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used
```
# <a name="c"></a>[<span data-ttu-id="361d1-155">C#</span><span class="sxs-lookup"><span data-stu-id="361d1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="361d1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="361d1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="361d1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="361d1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="361d1-158">Java</span><span class="sxs-lookup"><span data-stu-id="361d1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifieddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="361d1-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="361d1-159">Response</span></span>

><span data-ttu-id="361d1-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="361d1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
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
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3/thumbnails/0/small/thumbnailContent",
                "previewText": "Page-1",
                "containerWebUrl": "https://contoso.sharepoint.com/sites/Retail/Shared Documents/NC460 Sales",
                "containerDisplayName": "Retail",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Retail/_layouts/15/Doc.aspx?sourcedoc=%7BF4463999-4FB5-4F8B-9994-968C56353C5B%7D&file=Org%20Chart.vsdx&action=default&DefaultItemOpen=1",
                "id": "drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a><span data-ttu-id="361d1-162">Пример 2. Возвращаем недавно просмотрённые документы, которые пользователь, вписанный, мог изменить или не изменить.</span><span class="sxs-lookup"><span data-stu-id="361d1-162">Example 2: Return the most recently viewed documents that the signed-in user might or might not have modified</span></span> 

#### <a name="request"></a><span data-ttu-id="361d1-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="361d1-163">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="361d1-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="361d1-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[<span data-ttu-id="361d1-165">C#</span><span class="sxs-lookup"><span data-stu-id="361d1-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="361d1-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="361d1-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="361d1-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="361d1-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="361d1-168">Java</span><span class="sxs-lookup"><span data-stu-id="361d1-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifiedandvieweddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="361d1-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="361d1-169">Response</span></span>
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
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!ZOatQFjNPEyy-0guRSS0ho36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01NTE4NPQAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Executive Corner",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Exec",
                "id": "sites/contoso.sharepoint.com,40ade664-cd58-4c3c-b2fb-482e4524b486,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        }
    ]
}
```


