---
author: JeremyKelley
description: Изменение свойств ресурса listItem.
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0c67ca1ee4deeb793bde68713d0ad6a235a31144
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415379"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="f87bc-103">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="f87bc-103">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f87bc-104">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="f87bc-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f87bc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f87bc-105">Permissions</span></span>

<span data-ttu-id="f87bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f87bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f87bc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f87bc-108">Permission type</span></span>      | <span data-ttu-id="f87bc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f87bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f87bc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f87bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f87bc-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f87bc-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f87bc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f87bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87bc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f87bc-113">Not supported.</span></span>    |
|<span data-ttu-id="f87bc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f87bc-114">Application</span></span> | <span data-ttu-id="f87bc-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f87bc-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f87bc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f87bc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="f87bc-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f87bc-117">Optional request headers</span></span>

| <span data-ttu-id="f87bc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f87bc-118">Name</span></span>       | <span data-ttu-id="f87bc-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f87bc-119">Value</span></span> | <span data-ttu-id="f87bc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f87bc-120">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="f87bc-121">_if-match_</span><span class="sxs-lookup"><span data-stu-id="f87bc-121">_if-match_</span></span> | <span data-ttu-id="f87bc-122">etag</span><span class="sxs-lookup"><span data-stu-id="f87bc-122">etag</span></span>  | <span data-ttu-id="f87bc-123">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="f87bc-123">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="f87bc-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f87bc-124">Request body</span></span>

<span data-ttu-id="f87bc-125">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f87bc-125">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="f87bc-126">Пример</span><span class="sxs-lookup"><span data-stu-id="f87bc-126">Example</span></span>

<span data-ttu-id="f87bc-127">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="f87bc-127">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="f87bc-128">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="f87bc-128">All other values on the listItem are left alone.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="f87bc-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="f87bc-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f87bc-130">C#</span><span class="sxs-lookup"><span data-stu-id="f87bc-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f87bc-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f87bc-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f87bc-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f87bc-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f87bc-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f87bc-133">Response</span></span>

<span data-ttu-id="f87bc-134">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f87bc-134">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
}
-->
