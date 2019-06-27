---
author: JeremyKelley
ms.author: JeremyKelley
title: Обновление ресурса listItem
description: Изменение свойств ресурса **[listItem][]**.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: cbda0492ff0435e23e3bb33ceb75d3461d141a1a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271955"
---
# <a name="update-listitem"></a><span data-ttu-id="b2b30-103">Обновление ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="b2b30-103">Update listItem</span></span>

<span data-ttu-id="b2b30-104">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="b2b30-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2b30-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2b30-105">Permissions</span></span>

<span data-ttu-id="b2b30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b30-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2b30-108">Permission type</span></span>      | <span data-ttu-id="b2b30-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2b30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2b30-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2b30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2b30-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b30-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2b30-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2b30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2b30-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b30-113">Not supported.</span></span>    |
|<span data-ttu-id="b2b30-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2b30-114">Application</span></span> | <span data-ttu-id="b2b30-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b30-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2b30-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2b30-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b2b30-117">Изменение свойств ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="b2b30-117">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="b2b30-118">Изменение значений столбцов ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="b2b30-118">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="b2b30-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2b30-119">Optional request headers</span></span>

| <span data-ttu-id="b2b30-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b2b30-120">Name</span></span>       | <span data-ttu-id="b2b30-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2b30-121">Value</span></span> | <span data-ttu-id="b2b30-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b30-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="b2b30-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="b2b30-123">_if-match_</span></span> | <span data-ttu-id="b2b30-124">etag</span><span class="sxs-lookup"><span data-stu-id="b2b30-124">etag</span></span>  | <span data-ttu-id="b2b30-125">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="b2b30-125">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="b2b30-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2b30-126">Request body</span></span> 
<span data-ttu-id="b2b30-127">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b2b30-127">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="b2b30-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2b30-128">Response</span></span> 

<span data-ttu-id="b2b30-129">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [fieldValueSet][] для обновленного элемента списка в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b2b30-129">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="b2b30-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b2b30-130">Example</span></span>

<span data-ttu-id="b2b30-131">В следующем примере обновляются поля **Color** (Цвет) и **Quantity** (Количество) элемента списка с указанием новых значений.</span><span class="sxs-lookup"><span data-stu-id="b2b30-131">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="b2b30-132">Все остальные значения для ресурса **listItem** останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="b2b30-132">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="b2b30-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2b30-133">Request</span></span> 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

### <a name="response"></a><span data-ttu-id="b2b30-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2b30-134">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b2b30-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b2b30-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b2b30-136">C#</span><span class="sxs-lookup"><span data-stu-id="b2b30-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2b30-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2b30-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b2b30-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2b30-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
