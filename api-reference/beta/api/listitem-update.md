---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 074df35c54795002897b1d0d147944715c7c79df
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598030"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="a6679-102">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="a6679-102">Update an item in a list</span></span>

<span data-ttu-id="a6679-103">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="a6679-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6679-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6679-104">Permissions</span></span>

<span data-ttu-id="a6679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6679-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6679-107">Permission type</span></span>      | <span data-ttu-id="a6679-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6679-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6679-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6679-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a6679-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6679-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6679-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6679-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6679-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6679-112">Not supported.</span></span>    |
|<span data-ttu-id="a6679-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6679-113">Application</span></span> | <span data-ttu-id="a6679-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6679-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6679-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6679-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="a6679-116">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6679-116">Optional request headers</span></span>

| <span data-ttu-id="a6679-117">Имя</span><span class="sxs-lookup"><span data-stu-id="a6679-117">Name</span></span>       | <span data-ttu-id="a6679-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a6679-118">Value</span></span> | <span data-ttu-id="a6679-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a6679-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="a6679-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="a6679-120">_if-match_</span></span> | <span data-ttu-id="a6679-121">etag</span><span class="sxs-lookup"><span data-stu-id="a6679-121">etag</span></span>  | <span data-ttu-id="a6679-122">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="a6679-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="a6679-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6679-123">Request body</span></span>

<span data-ttu-id="a6679-124">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a6679-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="a6679-125">Пример</span><span class="sxs-lookup"><span data-stu-id="a6679-125">Example</span></span>

<span data-ttu-id="a6679-126">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="a6679-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="a6679-127">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="a6679-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="a6679-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6679-128">Response</span></span>

<span data-ttu-id="a6679-129">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a6679-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a6679-130">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="a6679-130">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6679-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6679-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
