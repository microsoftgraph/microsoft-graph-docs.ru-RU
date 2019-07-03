---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4849c3a4c2478ee21da0d64d8096377fd00eaef6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449157"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="bfb16-102">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="bfb16-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfb16-103">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="bfb16-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfb16-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfb16-104">Permissions</span></span>

<span data-ttu-id="bfb16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfb16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfb16-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfb16-107">Permission type</span></span>      | <span data-ttu-id="bfb16-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfb16-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfb16-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfb16-109">Delegated (work or school account)</span></span> | <span data-ttu-id="bfb16-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb16-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfb16-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfb16-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfb16-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfb16-112">Not supported.</span></span>    |
|<span data-ttu-id="bfb16-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfb16-113">Application</span></span> | <span data-ttu-id="bfb16-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb16-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfb16-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfb16-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="bfb16-116">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfb16-116">Optional request headers</span></span>

| <span data-ttu-id="bfb16-117">Имя</span><span class="sxs-lookup"><span data-stu-id="bfb16-117">Name</span></span>       | <span data-ttu-id="bfb16-118">Значение</span><span class="sxs-lookup"><span data-stu-id="bfb16-118">Value</span></span> | <span data-ttu-id="bfb16-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bfb16-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="bfb16-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="bfb16-120">_if-match_</span></span> | <span data-ttu-id="bfb16-121">etag</span><span class="sxs-lookup"><span data-stu-id="bfb16-121">etag</span></span>  | <span data-ttu-id="bfb16-122">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="bfb16-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="bfb16-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bfb16-123">Request body</span></span>

<span data-ttu-id="bfb16-124">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="bfb16-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="bfb16-125">Пример</span><span class="sxs-lookup"><span data-stu-id="bfb16-125">Example</span></span>

<span data-ttu-id="bfb16-126">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="bfb16-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="bfb16-127">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="bfb16-127">All other values on the listItem are left alone.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="bfb16-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb16-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bfb16-129">C#</span><span class="sxs-lookup"><span data-stu-id="bfb16-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfb16-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="bfb16-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bfb16-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bfb16-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="bfb16-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfb16-132">Response</span></span>

<span data-ttu-id="bfb16-133">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bfb16-133">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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
