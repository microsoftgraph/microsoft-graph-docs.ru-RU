---
author: JeremyKelley
title: Обновление ресурса listItem
description: Изменение свойств ресурса **[listItem][]**.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b1801539278f2a68bd7ebd3ab0cf505f9ecf1055
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474836"
---
# <a name="update-listitem"></a><span data-ttu-id="58e22-103">Обновление ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="58e22-103">Update listItem</span></span>

<span data-ttu-id="58e22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58e22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58e22-105">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="58e22-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="58e22-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58e22-106">Permissions</span></span>

<span data-ttu-id="58e22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e22-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58e22-109">Permission type</span></span>      | <span data-ttu-id="58e22-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58e22-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58e22-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58e22-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58e22-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e22-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="58e22-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58e22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e22-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e22-114">Not supported.</span></span>    |
|<span data-ttu-id="58e22-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58e22-115">Application</span></span> | <span data-ttu-id="58e22-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e22-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e22-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58e22-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="58e22-118">Изменение свойств ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="58e22-118">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="58e22-119">Изменение значений столбцов ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="58e22-119">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="58e22-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58e22-120">Optional request headers</span></span>

| <span data-ttu-id="58e22-121">Имя</span><span class="sxs-lookup"><span data-stu-id="58e22-121">Name</span></span>       | <span data-ttu-id="58e22-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58e22-122">Value</span></span> | <span data-ttu-id="58e22-123">Описание</span><span class="sxs-lookup"><span data-stu-id="58e22-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="58e22-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="58e22-124">_if-match_</span></span> | <span data-ttu-id="58e22-125">etag</span><span class="sxs-lookup"><span data-stu-id="58e22-125">etag</span></span>  | <span data-ttu-id="58e22-126">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="58e22-126">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="58e22-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58e22-127">Request body</span></span> 
<span data-ttu-id="58e22-128">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="58e22-128">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="58e22-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e22-129">Response</span></span> 

<span data-ttu-id="58e22-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [fieldValueSet][] для обновленного элемента списка в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58e22-130">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="58e22-131">Пример</span><span class="sxs-lookup"><span data-stu-id="58e22-131">Example</span></span>

<span data-ttu-id="58e22-132">В следующем примере обновляются поля **Color** (Цвет) и **Quantity** (Количество) элемента списка с указанием новых значений.</span><span class="sxs-lookup"><span data-stu-id="58e22-132">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="58e22-133">Все остальные значения для ресурса **listItem** останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="58e22-133">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="58e22-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e22-134">Request</span></span> 


# <a name="http"></a>[<span data-ttu-id="58e22-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="58e22-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="58e22-136">C#</span><span class="sxs-lookup"><span data-stu-id="58e22-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58e22-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58e22-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58e22-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58e22-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58e22-139">Java</span><span class="sxs-lookup"><span data-stu-id="58e22-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58e22-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e22-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

```http
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
} -->

