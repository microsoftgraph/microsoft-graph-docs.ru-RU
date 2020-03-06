---
author: JeremyKelley
ms.author: JeremyKelley
title: Получение ресурса listItem
description: Возвращает метаданные элемента в списке SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0d581732ab7a1fea6e5519ef0db0c289cd276d8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511707"
---
# <a name="get-listitem"></a><span data-ttu-id="13cd2-103">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="13cd2-103">Get listItem</span></span>

<span data-ttu-id="13cd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13cd2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13cd2-105">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="13cd2-105">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="13cd2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13cd2-108">Permissions</span></span>

<span data-ttu-id="13cd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13cd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13cd2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13cd2-111">Permission type</span></span>      | <span data-ttu-id="13cd2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13cd2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13cd2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13cd2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="13cd2-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13cd2-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="13cd2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13cd2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13cd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13cd2-116">Not supported.</span></span>    |
|<span data-ttu-id="13cd2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13cd2-117">Application</span></span> | <span data-ttu-id="13cd2-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13cd2-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13cd2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13cd2-119">HTTP request</span></span>

<span data-ttu-id="13cd2-120">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="13cd2-120">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="13cd2-121">Получение значений столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="13cd2-121">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="13cd2-122">Получение значений определенных столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="13cd2-122">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13cd2-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13cd2-123">Optional query parameters</span></span>
<span data-ttu-id="13cd2-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="13cd2-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13cd2-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13cd2-125">Request headers</span></span>

| <span data-ttu-id="13cd2-126">Имя</span><span class="sxs-lookup"><span data-stu-id="13cd2-126">Name</span></span>      |<span data-ttu-id="13cd2-127">Описание</span><span class="sxs-lookup"><span data-stu-id="13cd2-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13cd2-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13cd2-128">Authorization</span></span>  | <span data-ttu-id="13cd2-129">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="13cd2-129">Bearer {code}.</span></span> <span data-ttu-id="13cd2-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="13cd2-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13cd2-131">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="13cd2-131">Request body</span></span>

<span data-ttu-id="13cd2-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13cd2-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13cd2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cd2-133">Response</span></span> 

<span data-ttu-id="13cd2-134">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [item][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13cd2-134">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13cd2-135">Пример</span><span class="sxs-lookup"><span data-stu-id="13cd2-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="13cd2-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="13cd2-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="13cd2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="13cd2-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="13cd2-138">C#</span><span class="sxs-lookup"><span data-stu-id="13cd2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13cd2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13cd2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13cd2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13cd2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13cd2-141">Java</span><span class="sxs-lookup"><span data-stu-id="13cd2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="13cd2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cd2-142">Response</span></span>

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
