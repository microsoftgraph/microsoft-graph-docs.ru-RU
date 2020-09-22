---
author: JeremyKelley
description: Изменение свойств ресурса listItem.
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b696c2417168de43d43770789dd8fdaf58ef59e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062451"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="c1082-103">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="c1082-103">Update an item in a list</span></span>

<span data-ttu-id="c1082-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1082-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1082-105">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="c1082-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1082-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1082-106">Permissions</span></span>

<span data-ttu-id="c1082-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1082-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1082-109">Permission type</span></span>      | <span data-ttu-id="c1082-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1082-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1082-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1082-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1082-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1082-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1082-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1082-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1082-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1082-114">Not supported.</span></span>    |
|<span data-ttu-id="c1082-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1082-115">Application</span></span> | <span data-ttu-id="c1082-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1082-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1082-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1082-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="c1082-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1082-118">Optional request headers</span></span>

| <span data-ttu-id="c1082-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c1082-119">Name</span></span>       | <span data-ttu-id="c1082-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c1082-120">Value</span></span> | <span data-ttu-id="c1082-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c1082-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="c1082-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="c1082-122">_if-match_</span></span> | <span data-ttu-id="c1082-123">etag</span><span class="sxs-lookup"><span data-stu-id="c1082-123">etag</span></span>  | <span data-ttu-id="c1082-124">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="c1082-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="c1082-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1082-125">Request body</span></span>

<span data-ttu-id="c1082-126">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c1082-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="c1082-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c1082-127">Example</span></span>

<span data-ttu-id="c1082-128">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="c1082-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="c1082-129">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="c1082-129">All other values on the listItem are left alone.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c1082-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1082-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="c1082-131">C#</span><span class="sxs-lookup"><span data-stu-id="c1082-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1082-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1082-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1082-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1082-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="c1082-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1082-134">Response</span></span>

<span data-ttu-id="c1082-135">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1082-135">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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


