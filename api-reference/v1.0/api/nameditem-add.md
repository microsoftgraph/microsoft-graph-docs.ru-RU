---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: df9279c091fd2c69a95ebfad72dbee0aa472079b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576227"
---
# <a name="add-named-item"></a><span data-ttu-id="69ac5-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="69ac5-103">Add Named Item</span></span>

<span data-ttu-id="69ac5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ac5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69ac5-105">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="69ac5-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="69ac5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69ac5-106">Permissions</span></span>
<span data-ttu-id="69ac5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ac5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ac5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69ac5-109">Permission type</span></span>      | <span data-ttu-id="69ac5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69ac5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69ac5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69ac5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69ac5-112">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ac5-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="69ac5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69ac5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69ac5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69ac5-114">Not supported.</span></span>    |
|<span data-ttu-id="69ac5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="69ac5-115">Application</span></span> | <span data-ttu-id="69ac5-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ac5-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69ac5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69ac5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="69ac5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69ac5-118">Request headers</span></span>
| <span data-ttu-id="69ac5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="69ac5-119">Name</span></span>       | <span data-ttu-id="69ac5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69ac5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69ac5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69ac5-121">Authorization</span></span>  | <span data-ttu-id="69ac5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69ac5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69ac5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="69ac5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="69ac5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="69ac5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ac5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69ac5-127">Request body</span></span>
<span data-ttu-id="69ac5-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="69ac5-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69ac5-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="69ac5-129">Parameter</span></span>    | <span data-ttu-id="69ac5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69ac5-130">Type</span></span>   |<span data-ttu-id="69ac5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69ac5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69ac5-132">name</span><span class="sxs-lookup"><span data-stu-id="69ac5-132">name</span></span>|<span data-ttu-id="69ac5-133">string</span><span class="sxs-lookup"><span data-stu-id="69ac5-133">string</span></span>|<span data-ttu-id="69ac5-134">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="69ac5-134">The name of the named item.</span></span>|
|<span data-ttu-id="69ac5-135">ссылка</span><span class="sxs-lookup"><span data-stu-id="69ac5-135">reference</span></span>|<span data-ttu-id="69ac5-136">Json</span><span class="sxs-lookup"><span data-stu-id="69ac5-136">Json</span></span>|<span data-ttu-id="69ac5-137">Формула или диапазон, на который будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="69ac5-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="69ac5-138">comment</span><span class="sxs-lookup"><span data-stu-id="69ac5-138">comment</span></span>|<span data-ttu-id="69ac5-139">string</span><span class="sxs-lookup"><span data-stu-id="69ac5-139">string</span></span>|<span data-ttu-id="69ac5-140">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="69ac5-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="69ac5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="69ac5-141">Response</span></span>

<span data-ttu-id="69ac5-142">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект WorkbookNamedItem](../resources/nameditem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="69ac5-142">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="69ac5-143">Пример</span><span class="sxs-lookup"><span data-stu-id="69ac5-143">Example</span></span>
<span data-ttu-id="69ac5-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="69ac5-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="69ac5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="69ac5-145">Request</span></span>
<span data-ttu-id="69ac5-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69ac5-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69ac5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="69ac5-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
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
# <a name="c"></a>[<span data-ttu-id="69ac5-148">C#</span><span class="sxs-lookup"><span data-stu-id="69ac5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69ac5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69ac5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69ac5-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69ac5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69ac5-151">Java</span><span class="sxs-lookup"><span data-stu-id="69ac5-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="69ac5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="69ac5-152">Response</span></span>
<span data-ttu-id="69ac5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69ac5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

