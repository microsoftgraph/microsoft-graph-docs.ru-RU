---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: b08abe6b4f5deb90c55b2452bb785157fec95cfe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810827"
---
# <a name="add-named-item"></a><span data-ttu-id="9d334-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="9d334-103">Add Named Item</span></span>

<span data-ttu-id="9d334-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d334-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d334-105">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="9d334-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d334-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d334-106">Permissions</span></span>
<span data-ttu-id="9d334-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d334-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d334-109">Permission type</span></span>      | <span data-ttu-id="9d334-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d334-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d334-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d334-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d334-112">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d334-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="9d334-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d334-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d334-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d334-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d334-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d334-115">Application</span></span> | <span data-ttu-id="9d334-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d334-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d334-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d334-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="9d334-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d334-118">Request headers</span></span>
| <span data-ttu-id="9d334-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9d334-119">Name</span></span>       | <span data-ttu-id="9d334-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9d334-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d334-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d334-121">Authorization</span></span>  | <span data-ttu-id="9d334-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d334-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d334-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9d334-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9d334-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9d334-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d334-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d334-127">Request body</span></span>
<span data-ttu-id="9d334-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9d334-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9d334-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="9d334-129">Parameter</span></span>    | <span data-ttu-id="9d334-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9d334-130">Type</span></span>   |<span data-ttu-id="9d334-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9d334-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d334-132">name</span><span class="sxs-lookup"><span data-stu-id="9d334-132">name</span></span>|<span data-ttu-id="9d334-133">string</span><span class="sxs-lookup"><span data-stu-id="9d334-133">string</span></span>|<span data-ttu-id="9d334-134">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="9d334-134">The name of the named item.</span></span>|
|<span data-ttu-id="9d334-135">ссылка</span><span class="sxs-lookup"><span data-stu-id="9d334-135">reference</span></span>|<span data-ttu-id="9d334-136">string</span><span class="sxs-lookup"><span data-stu-id="9d334-136">string</span></span>|<span data-ttu-id="9d334-137">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="9d334-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="9d334-138">comment</span><span class="sxs-lookup"><span data-stu-id="9d334-138">comment</span></span>|<span data-ttu-id="9d334-139">string</span><span class="sxs-lookup"><span data-stu-id="9d334-139">string</span></span>|<span data-ttu-id="9d334-140">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="9d334-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="9d334-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d334-141">Response</span></span>

<span data-ttu-id="9d334-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукнамедитем](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d334-142">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d334-143">Пример</span><span class="sxs-lookup"><span data-stu-id="9d334-143">Example</span></span>
<span data-ttu-id="9d334-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9d334-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9d334-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d334-145">Request</span></span>
<span data-ttu-id="9d334-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d334-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d334-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d334-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9d334-148">C#</span><span class="sxs-lookup"><span data-stu-id="9d334-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d334-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d334-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d334-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d334-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9d334-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d334-151">Response</span></span>
<span data-ttu-id="9d334-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d334-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
