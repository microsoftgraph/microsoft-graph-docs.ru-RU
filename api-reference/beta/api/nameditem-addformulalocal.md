---
title: Add Named Item FormulaLocal
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 02572edce528f12162d0b0a41b169fc8cc9065d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062383"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="8d316-103">Add Named Item FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="8d316-103">Add Named Item FormulaLocal</span></span>

<span data-ttu-id="8d316-104">Пространство имен: Microsoft. Graph добавляет новое имя в коллекцию заданной области, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="8d316-104">Namespace: microsoft.graph Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d316-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d316-105">Permissions</span></span>
<span data-ttu-id="8d316-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d316-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d316-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d316-108">Permission type</span></span>      | <span data-ttu-id="8d316-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d316-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d316-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d316-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d316-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d316-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="8d316-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d316-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d316-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d316-113">Not supported.</span></span>    |
|<span data-ttu-id="8d316-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d316-114">Application</span></span> | <span data-ttu-id="8d316-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d316-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d316-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d316-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="8d316-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d316-117">Request headers</span></span>
| <span data-ttu-id="8d316-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8d316-118">Name</span></span>       | <span data-ttu-id="8d316-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8d316-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d316-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d316-120">Authorization</span></span>  | <span data-ttu-id="8d316-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d316-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d316-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8d316-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8d316-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8d316-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d316-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d316-126">Request body</span></span>
<span data-ttu-id="8d316-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8d316-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d316-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="8d316-128">Parameter</span></span>    | <span data-ttu-id="8d316-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8d316-129">Type</span></span>   |<span data-ttu-id="8d316-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8d316-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d316-131">name</span><span class="sxs-lookup"><span data-stu-id="8d316-131">name</span></span>|<span data-ttu-id="8d316-132">string</span><span class="sxs-lookup"><span data-stu-id="8d316-132">string</span></span>|<span data-ttu-id="8d316-133">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="8d316-133">The name of the named item.</span></span>|
|<span data-ttu-id="8d316-134">формула</span><span class="sxs-lookup"><span data-stu-id="8d316-134">formula</span></span>|<span data-ttu-id="8d316-135">string</span><span class="sxs-lookup"><span data-stu-id="8d316-135">string</span></span>|<span data-ttu-id="8d316-136">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="8d316-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="8d316-137">comment</span><span class="sxs-lookup"><span data-stu-id="8d316-137">comment</span></span>|<span data-ttu-id="8d316-138">string</span><span class="sxs-lookup"><span data-stu-id="8d316-138">string</span></span>|<span data-ttu-id="8d316-139">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="8d316-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="8d316-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d316-140">Response</span></span>

<span data-ttu-id="8d316-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [NamedItem](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d316-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d316-142">Пример</span><span class="sxs-lookup"><span data-stu-id="8d316-142">Example</span></span>
<span data-ttu-id="8d316-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8d316-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8d316-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d316-144">Request</span></span>
<span data-ttu-id="8d316-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d316-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d316-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d316-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
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
# <a name="c"></a>[<span data-ttu-id="8d316-147">C#</span><span class="sxs-lookup"><span data-stu-id="8d316-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d316-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d316-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d316-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d316-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8d316-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d316-150">Response</span></span>
<span data-ttu-id="8d316-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d316-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


