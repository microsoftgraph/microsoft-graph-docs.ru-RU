---
author: JeremyKelley
ms.author: JeremyKelley
title: Получение ресурса listItem
description: Возвращает метаданные элемента в списке SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e2d441bb306a6614cdc27f5dff79bd55377b0459
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057292"
---
# <a name="get-listitem"></a><span data-ttu-id="b928e-103">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="b928e-103">Get listItem</span></span>

<span data-ttu-id="b928e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b928e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b928e-105">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="b928e-105">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="b928e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b928e-108">Permissions</span></span>

<span data-ttu-id="b928e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b928e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b928e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b928e-111">Permission type</span></span>      | <span data-ttu-id="b928e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b928e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b928e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b928e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b928e-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b928e-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b928e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b928e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b928e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b928e-116">Not supported.</span></span>    |
|<span data-ttu-id="b928e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b928e-117">Application</span></span> | <span data-ttu-id="b928e-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b928e-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b928e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b928e-119">HTTP request</span></span>

<span data-ttu-id="b928e-120">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="b928e-120">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="b928e-121">Получение значений столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="b928e-121">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="b928e-122">Получение значений определенных столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="b928e-122">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b928e-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b928e-123">Optional query parameters</span></span>
<span data-ttu-id="b928e-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b928e-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b928e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b928e-125">Request headers</span></span>

| <span data-ttu-id="b928e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b928e-126">Name</span></span>      |<span data-ttu-id="b928e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b928e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b928e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b928e-128">Authorization</span></span>  | <span data-ttu-id="b928e-129">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="b928e-129">Bearer {code}.</span></span> <span data-ttu-id="b928e-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b928e-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b928e-131">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="b928e-131">Request body</span></span>

<span data-ttu-id="b928e-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b928e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b928e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b928e-133">Response</span></span> 

<span data-ttu-id="b928e-134">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [item][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b928e-134">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b928e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b928e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="b928e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b928e-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b928e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b928e-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="b928e-138">C#</span><span class="sxs-lookup"><span data-stu-id="b928e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b928e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b928e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b928e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b928e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b928e-141">Java</span><span class="sxs-lookup"><span data-stu-id="b928e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b928e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b928e-142">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
} -->

