---
title: Обновление объекта rangeFill
description: Обновление свойств объекта rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 08dcc5f9181354f394741fffa036375a865b53b7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034968"
---
# <a name="update-rangefill"></a><span data-ttu-id="0b82c-103">Обновление объекта rangeFill</span><span class="sxs-lookup"><span data-stu-id="0b82c-103">Update rangefill</span></span>

<span data-ttu-id="0b82c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b82c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b82c-105">Обновление свойств объекта rangefill.</span><span class="sxs-lookup"><span data-stu-id="0b82c-105">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b82c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b82c-106">Permissions</span></span>
<span data-ttu-id="0b82c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b82c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b82c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b82c-109">Permission type</span></span>      | <span data-ttu-id="0b82c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b82c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b82c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b82c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b82c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b82c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b82c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b82c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b82c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b82c-114">Not supported.</span></span>    |
|<span data-ttu-id="0b82c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b82c-115">Application</span></span> | <span data-ttu-id="0b82c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b82c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b82c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b82c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/fill
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="0b82c-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b82c-118">Optional request headers</span></span>
| <span data-ttu-id="0b82c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b82c-119">Name</span></span>       | <span data-ttu-id="0b82c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0b82c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0b82c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b82c-121">Authorization</span></span>  | <span data-ttu-id="0b82c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b82c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b82c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b82c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b82c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0b82c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b82c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b82c-127">Request body</span></span>
<span data-ttu-id="0b82c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0b82c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b82c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b82c-131">Property</span></span>     | <span data-ttu-id="0b82c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0b82c-132">Type</span></span>   |<span data-ttu-id="0b82c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0b82c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b82c-134">color</span><span class="sxs-lookup"><span data-stu-id="0b82c-134">color</span></span>|<span data-ttu-id="0b82c-135">string</span><span class="sxs-lookup"><span data-stu-id="0b82c-135">string</span></span>|<span data-ttu-id="0b82c-136">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="0b82c-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="0b82c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b82c-137">Response</span></span>

<span data-ttu-id="0b82c-138">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookRangeFill](../resources/rangefill.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0b82c-138">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b82c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0b82c-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b82c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b82c-140">Request</span></span>
<span data-ttu-id="0b82c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b82c-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b82c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b82c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="0b82c-143">C#</span><span class="sxs-lookup"><span data-stu-id="0b82c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b82c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b82c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b82c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b82c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b82c-146">Java</span><span class="sxs-lookup"><span data-stu-id="0b82c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b82c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b82c-147">Response</span></span>
<span data-ttu-id="0b82c-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b82c-148">Here is an example of the response.</span></span> <span data-ttu-id="0b82c-149">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b82c-149">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

