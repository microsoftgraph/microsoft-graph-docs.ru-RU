---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 360f10662cda93a692c3cdc082dce96cad5e2261
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949776"
---
# <a name="add-named-item"></a><span data-ttu-id="0cbc7-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="0cbc7-103">Add Named Item</span></span>

<span data-ttu-id="0cbc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cbc7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cbc7-105">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cbc7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cbc7-106">Permissions</span></span>
<span data-ttu-id="0cbc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cbc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cbc7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cbc7-109">Permission type</span></span>      | <span data-ttu-id="0cbc7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cbc7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cbc7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cbc7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0cbc7-112">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cbc7-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="0cbc7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cbc7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cbc7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-114">Not supported.</span></span>    |
|<span data-ttu-id="0cbc7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cbc7-115">Application</span></span> | <span data-ttu-id="0cbc7-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cbc7-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cbc7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cbc7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="0cbc7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cbc7-118">Request headers</span></span>
| <span data-ttu-id="0cbc7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0cbc7-119">Name</span></span>       | <span data-ttu-id="0cbc7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0cbc7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0cbc7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cbc7-121">Authorization</span></span>  | <span data-ttu-id="0cbc7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0cbc7-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0cbc7-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0cbc7-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cbc7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cbc7-127">Request body</span></span>
<span data-ttu-id="0cbc7-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0cbc7-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="0cbc7-129">Parameter</span></span>    | <span data-ttu-id="0cbc7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0cbc7-130">Type</span></span>   |<span data-ttu-id="0cbc7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0cbc7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cbc7-132">name</span><span class="sxs-lookup"><span data-stu-id="0cbc7-132">name</span></span>|<span data-ttu-id="0cbc7-133">string</span><span class="sxs-lookup"><span data-stu-id="0cbc7-133">string</span></span>|<span data-ttu-id="0cbc7-134">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-134">The name of the named item.</span></span>|
|<span data-ttu-id="0cbc7-135">ссылка</span><span class="sxs-lookup"><span data-stu-id="0cbc7-135">reference</span></span>|<span data-ttu-id="0cbc7-136">Json</span><span class="sxs-lookup"><span data-stu-id="0cbc7-136">Json</span></span>|<span data-ttu-id="0cbc7-137">Формула или диапазон, на который будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="0cbc7-138">comment</span><span class="sxs-lookup"><span data-stu-id="0cbc7-138">comment</span></span>|<span data-ttu-id="0cbc7-139">string</span><span class="sxs-lookup"><span data-stu-id="0cbc7-139">string</span></span>|<span data-ttu-id="0cbc7-140">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="0cbc7-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="0cbc7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cbc7-141">Response</span></span>

<span data-ttu-id="0cbc7-142">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект WorkbookNamedItem](../resources/nameditem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-142">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="0cbc7-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0cbc7-143">Example</span></span>
<span data-ttu-id="0cbc7-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0cbc7-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cbc7-145">Request</span></span>
<span data-ttu-id="0cbc7-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cbc7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cbc7-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0cbc7-148">C#</span><span class="sxs-lookup"><span data-stu-id="0cbc7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cbc7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cbc7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cbc7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cbc7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cbc7-151">Java</span><span class="sxs-lookup"><span data-stu-id="0cbc7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0cbc7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cbc7-152">Response</span></span>
<span data-ttu-id="0cbc7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cbc7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Warning: NamedItemcollection_add/value:
      Schemas type was 'Custom' which is not supported. Add a resource type to the definition of property: value"
  ],
  "tocPath": ""
}-->

