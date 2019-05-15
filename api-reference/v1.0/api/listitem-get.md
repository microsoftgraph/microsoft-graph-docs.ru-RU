---
author: JeremyKelley
ms.author: JeremyKelley
title: Получение ресурса listItem
description: Возвращает метаданные элемента в списке SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a498947002247541bebf4fc7cd24147a0ca0df7a
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968788"
---
# <a name="get-listitem"></a><span data-ttu-id="c4a9e-103">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="c4a9e-103">Get listItem</span></span>

<span data-ttu-id="c4a9e-104">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="c4a9e-104">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="c4a9e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4a9e-107">Permissions</span></span>

<span data-ttu-id="c4a9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a9e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4a9e-110">Permission type</span></span>      | <span data-ttu-id="c4a9e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4a9e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4a9e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4a9e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4a9e-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a9e-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4a9e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4a9e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4a9e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4a9e-115">Not supported.</span></span>    |
|<span data-ttu-id="c4a9e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4a9e-116">Application</span></span> | <span data-ttu-id="c4a9e-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a9e-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4a9e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4a9e-118">HTTP request</span></span>

<span data-ttu-id="c4a9e-119">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="c4a9e-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="c4a9e-120">Получение значений столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="c4a9e-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="c4a9e-121">Получение значений определенных столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="c4a9e-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4a9e-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4a9e-122">Optional query parameters</span></span>
<span data-ttu-id="c4a9e-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c4a9e-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4a9e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4a9e-124">Request headers</span></span>

| <span data-ttu-id="c4a9e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="c4a9e-125">Name</span></span>      |<span data-ttu-id="c4a9e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c4a9e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4a9e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4a9e-127">Authorization</span></span>  | <span data-ttu-id="c4a9e-128">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="c4a9e-128">Bearer {code}.</span></span> <span data-ttu-id="c4a9e-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c4a9e-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a9e-130">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="c4a9e-130">Request body</span></span>

<span data-ttu-id="c4a9e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4a9e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a9e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4a9e-132">Response</span></span> 

<span data-ttu-id="c4a9e-133">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [item][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4a9e-133">If successful, this method returns a `200 OK` response code and an [attachment][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a9e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c4a9e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4a9e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4a9e-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="c4a9e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4a9e-136">Response</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="c4a9e-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c4a9e-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c4a9e-138">C#</span><span class="sxs-lookup"><span data-stu-id="c4a9e-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4a9e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4a9e-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
