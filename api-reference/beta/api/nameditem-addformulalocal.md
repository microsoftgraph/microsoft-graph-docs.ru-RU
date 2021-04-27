---
title: Add Named Item FormulaLocal
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 24773d20df7640ad50263cfbc2f395b0bc8cfa77
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052140"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="4c443-103">Add Named Item FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="4c443-103">Add Named Item FormulaLocal</span></span>

<span data-ttu-id="4c443-104">Пространство имен: microsoft.graph добавляет новое имя в коллекцию данной области с помощью локалиа пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="4c443-104">Namespace: microsoft.graph Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c443-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c443-105">Permissions</span></span>
<span data-ttu-id="4c443-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c443-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c443-108">Permission type</span></span>      | <span data-ttu-id="4c443-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c443-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c443-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c443-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c443-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c443-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="4c443-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c443-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c443-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c443-113">Not supported.</span></span>    |
|<span data-ttu-id="4c443-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="4c443-114">Application</span></span> | <span data-ttu-id="4c443-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c443-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c443-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c443-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="4c443-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c443-117">Request headers</span></span>
| <span data-ttu-id="4c443-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4c443-118">Name</span></span>       | <span data-ttu-id="4c443-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4c443-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4c443-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c443-120">Authorization</span></span>  | <span data-ttu-id="4c443-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c443-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c443-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4c443-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4c443-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4c443-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c443-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c443-126">Request body</span></span>
<span data-ttu-id="4c443-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4c443-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c443-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c443-128">Parameter</span></span>    | <span data-ttu-id="4c443-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4c443-129">Type</span></span>   |<span data-ttu-id="4c443-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4c443-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c443-131">name</span><span class="sxs-lookup"><span data-stu-id="4c443-131">name</span></span>|<span data-ttu-id="4c443-132">string</span><span class="sxs-lookup"><span data-stu-id="4c443-132">string</span></span>|<span data-ttu-id="4c443-133">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="4c443-133">The name of the named item.</span></span>|
|<span data-ttu-id="4c443-134">формула</span><span class="sxs-lookup"><span data-stu-id="4c443-134">formula</span></span>|<span data-ttu-id="4c443-135">string</span><span class="sxs-lookup"><span data-stu-id="4c443-135">string</span></span>|<span data-ttu-id="4c443-136">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="4c443-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="4c443-137">comment</span><span class="sxs-lookup"><span data-stu-id="4c443-137">comment</span></span>|<span data-ttu-id="4c443-138">string</span><span class="sxs-lookup"><span data-stu-id="4c443-138">string</span></span>|<span data-ttu-id="4c443-139">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="4c443-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="4c443-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c443-140">Response</span></span>

<span data-ttu-id="4c443-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [NamedItem](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c443-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c443-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4c443-142">Example</span></span>
<span data-ttu-id="4c443-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4c443-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4c443-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c443-144">Request</span></span>
<span data-ttu-id="4c443-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c443-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4c443-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c443-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```
# <a name="c"></a>[<span data-ttu-id="4c443-147">C#</span><span class="sxs-lookup"><span data-stu-id="4c443-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c443-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c443-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c443-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c443-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c443-150">Java</span><span class="sxs-lookup"><span data-stu-id="4c443-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c443-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c443-151">Response</span></span>
<span data-ttu-id="4c443-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c443-152">Here is an example of the response.</span></span> <span data-ttu-id="4c443-153">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c443-153">Note: The response object shown here might be shortened for readability.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->


