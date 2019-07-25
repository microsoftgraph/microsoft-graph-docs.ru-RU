---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
ms.openlocfilehash: 2657326b774d111adbb0012f983eb99acccb15f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879278"
---
# <a name="add-named-item"></a><span data-ttu-id="79907-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="79907-103">Add Named Item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79907-104">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="79907-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="79907-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79907-105">Permissions</span></span>
<span data-ttu-id="79907-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79907-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79907-108">Permission type</span></span>      | <span data-ttu-id="79907-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79907-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79907-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79907-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79907-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="79907-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="79907-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79907-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79907-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79907-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79907-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79907-114">Application</span></span> | <span data-ttu-id="79907-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="79907-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79907-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79907-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="79907-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79907-117">Request headers</span></span>
| <span data-ttu-id="79907-118">Имя</span><span class="sxs-lookup"><span data-stu-id="79907-118">Name</span></span>       | <span data-ttu-id="79907-119">Описание</span><span class="sxs-lookup"><span data-stu-id="79907-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79907-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79907-120">Authorization</span></span>  | <span data-ttu-id="79907-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79907-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79907-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="79907-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="79907-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="79907-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79907-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79907-126">Request body</span></span>
<span data-ttu-id="79907-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="79907-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79907-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="79907-128">Parameter</span></span>    | <span data-ttu-id="79907-129">Тип</span><span class="sxs-lookup"><span data-stu-id="79907-129">Type</span></span>   |<span data-ttu-id="79907-130">Описание</span><span class="sxs-lookup"><span data-stu-id="79907-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79907-131">name</span><span class="sxs-lookup"><span data-stu-id="79907-131">name</span></span>|<span data-ttu-id="79907-132">string</span><span class="sxs-lookup"><span data-stu-id="79907-132">string</span></span>|<span data-ttu-id="79907-133">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="79907-133">The name of the named item.</span></span>|
|<span data-ttu-id="79907-134">ссылка</span><span class="sxs-lookup"><span data-stu-id="79907-134">reference</span></span>|<span data-ttu-id="79907-135">string</span><span class="sxs-lookup"><span data-stu-id="79907-135">string</span></span>|<span data-ttu-id="79907-136">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="79907-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="79907-137">примечание</span><span class="sxs-lookup"><span data-stu-id="79907-137">comment</span></span>|<span data-ttu-id="79907-138">string</span><span class="sxs-lookup"><span data-stu-id="79907-138">string</span></span>|<span data-ttu-id="79907-139">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="79907-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="79907-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="79907-140">Response</span></span>

<span data-ttu-id="79907-141">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукнамедитем](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79907-141">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79907-142">Пример</span><span class="sxs-lookup"><span data-stu-id="79907-142">Example</span></span>
<span data-ttu-id="79907-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="79907-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="79907-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="79907-144">Request</span></span>
<span data-ttu-id="79907-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79907-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79907-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="79907-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79907-147">C#</span><span class="sxs-lookup"><span data-stu-id="79907-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79907-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="79907-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79907-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="79907-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79907-150">Java</span><span class="sxs-lookup"><span data-stu-id="79907-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79907-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="79907-151">Response</span></span>
<span data-ttu-id="79907-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79907-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
