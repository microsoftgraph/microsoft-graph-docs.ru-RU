---
author: JeremyKelley
ms.author: JeremyKelley
title: Получение ресурса listItem
description: Возвращает метаданные элемента в списке SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 458b8e71f8561c6a96177bac38c8ed450110ee24
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370682"
---
# <a name="get-listitem"></a><span data-ttu-id="378cc-103">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="378cc-103">Get listItem</span></span>

<span data-ttu-id="378cc-104">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="378cc-104">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="378cc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="378cc-107">Permissions</span></span>

<span data-ttu-id="378cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="378cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="378cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="378cc-110">Permission type</span></span>      | <span data-ttu-id="378cc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="378cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="378cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="378cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="378cc-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="378cc-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="378cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="378cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="378cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="378cc-115">Not supported.</span></span>    |
|<span data-ttu-id="378cc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="378cc-116">Application</span></span> | <span data-ttu-id="378cc-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="378cc-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="378cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="378cc-118">HTTP request</span></span>

<span data-ttu-id="378cc-119">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="378cc-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="378cc-120">Получение значений столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="378cc-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="378cc-121">Получение значений определенных столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="378cc-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="378cc-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="378cc-122">Optional query parameters</span></span>
<span data-ttu-id="378cc-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="378cc-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="378cc-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="378cc-124">Request headers</span></span>

| <span data-ttu-id="378cc-125">Имя</span><span class="sxs-lookup"><span data-stu-id="378cc-125">Name</span></span>      |<span data-ttu-id="378cc-126">Описание</span><span class="sxs-lookup"><span data-stu-id="378cc-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="378cc-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="378cc-127">Authorization</span></span>  | <span data-ttu-id="378cc-128">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="378cc-128">Bearer {code}.</span></span> <span data-ttu-id="378cc-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="378cc-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="378cc-130">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="378cc-130">Request body</span></span>

<span data-ttu-id="378cc-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="378cc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="378cc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="378cc-132">Response</span></span> 

<span data-ttu-id="378cc-133">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [item][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="378cc-133">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="378cc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="378cc-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="378cc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="378cc-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="378cc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="378cc-136">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="378cc-137">C#</span><span class="sxs-lookup"><span data-stu-id="378cc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="378cc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="378cc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="378cc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="378cc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="378cc-140">Java</span><span class="sxs-lookup"><span data-stu-id="378cc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="378cc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="378cc-141">Response</span></span>

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
