---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9996d9974a0e98a86e3770228b2bd03495e30894
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108230"
---
# <a name="add-named-item"></a><span data-ttu-id="d18ac-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="d18ac-103">Add Named Item</span></span>

<span data-ttu-id="d18ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d18ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d18ac-105">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="d18ac-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="d18ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d18ac-106">Permissions</span></span>
<span data-ttu-id="d18ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d18ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d18ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d18ac-109">Permission type</span></span>      | <span data-ttu-id="d18ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d18ac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d18ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d18ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d18ac-112">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d18ac-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="d18ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d18ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d18ac-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d18ac-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d18ac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d18ac-115">Application</span></span> | <span data-ttu-id="d18ac-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d18ac-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d18ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d18ac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="d18ac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d18ac-118">Request headers</span></span>
| <span data-ttu-id="d18ac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d18ac-119">Name</span></span>       | <span data-ttu-id="d18ac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d18ac-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d18ac-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d18ac-121">Authorization</span></span>  | <span data-ttu-id="d18ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d18ac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d18ac-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d18ac-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d18ac-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d18ac-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d18ac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d18ac-127">Request body</span></span>
<span data-ttu-id="d18ac-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d18ac-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d18ac-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="d18ac-129">Parameter</span></span>    | <span data-ttu-id="d18ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d18ac-130">Type</span></span>   |<span data-ttu-id="d18ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d18ac-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d18ac-132">name</span><span class="sxs-lookup"><span data-stu-id="d18ac-132">name</span></span>|<span data-ttu-id="d18ac-133">string</span><span class="sxs-lookup"><span data-stu-id="d18ac-133">string</span></span>|<span data-ttu-id="d18ac-134">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="d18ac-134">The name of the named item.</span></span>|
|<span data-ttu-id="d18ac-135">ссылка</span><span class="sxs-lookup"><span data-stu-id="d18ac-135">reference</span></span>|<span data-ttu-id="d18ac-136">string</span><span class="sxs-lookup"><span data-stu-id="d18ac-136">string</span></span>|<span data-ttu-id="d18ac-137">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="d18ac-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="d18ac-138">comment</span><span class="sxs-lookup"><span data-stu-id="d18ac-138">comment</span></span>|<span data-ttu-id="d18ac-139">string</span><span class="sxs-lookup"><span data-stu-id="d18ac-139">string</span></span>|<span data-ttu-id="d18ac-140">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="d18ac-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="d18ac-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d18ac-141">Response</span></span>

<span data-ttu-id="d18ac-142">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукнамедитем](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d18ac-142">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d18ac-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d18ac-143">Example</span></span>
<span data-ttu-id="d18ac-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d18ac-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d18ac-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d18ac-145">Request</span></span>
<span data-ttu-id="d18ac-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d18ac-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d18ac-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d18ac-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d18ac-148">C#</span><span class="sxs-lookup"><span data-stu-id="d18ac-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d18ac-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d18ac-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d18ac-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d18ac-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d18ac-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d18ac-151">Response</span></span>
<span data-ttu-id="d18ac-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d18ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
