---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 814106eed33c422282e76f5ed08961e0ed5a5a23
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786350"
---
# <a name="add-named-item"></a><span data-ttu-id="c6c04-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="c6c04-103">Add Named Item</span></span>

<span data-ttu-id="c6c04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6c04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6c04-105">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="c6c04-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6c04-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6c04-106">Permissions</span></span>
<span data-ttu-id="c6c04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6c04-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6c04-109">Permission type</span></span>      | <span data-ttu-id="c6c04-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6c04-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6c04-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6c04-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6c04-112">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6c04-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="c6c04-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6c04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6c04-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6c04-114">Not supported.</span></span>    |
|<span data-ttu-id="c6c04-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6c04-115">Application</span></span> | <span data-ttu-id="c6c04-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6c04-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6c04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6c04-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="c6c04-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6c04-118">Request headers</span></span>
| <span data-ttu-id="c6c04-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c6c04-119">Name</span></span>       | <span data-ttu-id="c6c04-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c6c04-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6c04-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6c04-121">Authorization</span></span>  | <span data-ttu-id="c6c04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6c04-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6c04-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c6c04-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c6c04-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c6c04-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6c04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6c04-127">Request body</span></span>
<span data-ttu-id="c6c04-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c6c04-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c6c04-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="c6c04-129">Parameter</span></span>    | <span data-ttu-id="c6c04-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c6c04-130">Type</span></span>   |<span data-ttu-id="c6c04-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c6c04-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6c04-132">name</span><span class="sxs-lookup"><span data-stu-id="c6c04-132">name</span></span>|<span data-ttu-id="c6c04-133">string</span><span class="sxs-lookup"><span data-stu-id="c6c04-133">string</span></span>|<span data-ttu-id="c6c04-134">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="c6c04-134">The name of the named item.</span></span>|
|<span data-ttu-id="c6c04-135">ссылка</span><span class="sxs-lookup"><span data-stu-id="c6c04-135">reference</span></span>|<span data-ttu-id="c6c04-136">Json</span><span class="sxs-lookup"><span data-stu-id="c6c04-136">Json</span></span>|<span data-ttu-id="c6c04-137">Формула или диапазон, на который будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="c6c04-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="c6c04-138">comment</span><span class="sxs-lookup"><span data-stu-id="c6c04-138">comment</span></span>|<span data-ttu-id="c6c04-139">string</span><span class="sxs-lookup"><span data-stu-id="c6c04-139">string</span></span>|<span data-ttu-id="c6c04-140">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="c6c04-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="c6c04-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6c04-141">Response</span></span>

<span data-ttu-id="c6c04-142">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект WorkbookNamedItem](../resources/nameditem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c6c04-142">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c6c04-143">Пример</span><span class="sxs-lookup"><span data-stu-id="c6c04-143">Example</span></span>
<span data-ttu-id="c6c04-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c6c04-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c6c04-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6c04-145">Request</span></span>
<span data-ttu-id="c6c04-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6c04-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6c04-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6c04-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```
# <a name="c"></a>[<span data-ttu-id="c6c04-148">C#</span><span class="sxs-lookup"><span data-stu-id="c6c04-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6c04-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6c04-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6c04-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6c04-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6c04-151">Java</span><span class="sxs-lookup"><span data-stu-id="c6c04-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c6c04-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6c04-152">Response</span></span>
<span data-ttu-id="c6c04-p104">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c6c04-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [],
  "tocPath": ""
}-->

