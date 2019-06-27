---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f365331b5941da48178194c9b02f61aaf1893ed6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264528"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="60821-102">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="60821-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60821-103">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="60821-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="60821-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60821-104">Permissions</span></span>

<span data-ttu-id="60821-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60821-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60821-107">Permission type</span></span>      | <span data-ttu-id="60821-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60821-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60821-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60821-109">Delegated (work or school account)</span></span> | <span data-ttu-id="60821-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60821-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="60821-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60821-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60821-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60821-112">Not supported.</span></span>    |
|<span data-ttu-id="60821-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60821-113">Application</span></span> | <span data-ttu-id="60821-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60821-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60821-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60821-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="60821-116">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60821-116">Optional request headers</span></span>

| <span data-ttu-id="60821-117">Имя</span><span class="sxs-lookup"><span data-stu-id="60821-117">Name</span></span>       | <span data-ttu-id="60821-118">Значение</span><span class="sxs-lookup"><span data-stu-id="60821-118">Value</span></span> | <span data-ttu-id="60821-119">Описание</span><span class="sxs-lookup"><span data-stu-id="60821-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="60821-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="60821-120">_if-match_</span></span> | <span data-ttu-id="60821-121">etag</span><span class="sxs-lookup"><span data-stu-id="60821-121">etag</span></span>  | <span data-ttu-id="60821-122">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="60821-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="60821-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60821-123">Request body</span></span>

<span data-ttu-id="60821-124">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="60821-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="60821-125">Пример</span><span class="sxs-lookup"><span data-stu-id="60821-125">Example</span></span>

<span data-ttu-id="60821-126">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="60821-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="60821-127">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="60821-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="60821-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="60821-128">Response</span></span>

<span data-ttu-id="60821-129">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="60821-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="60821-130">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="60821-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="60821-131">C#</span><span class="sxs-lookup"><span data-stu-id="60821-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60821-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="60821-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="60821-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="60821-133">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
