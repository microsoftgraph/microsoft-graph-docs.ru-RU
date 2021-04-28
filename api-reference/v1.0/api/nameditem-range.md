---
title: 'NamedItem: Range'
description: Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 16f692af808b66e09952322f329e4c09a6ceb47f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039365"
---
# <a name="nameditem-range"></a><span data-ttu-id="99730-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="99730-104">NamedItem: Range</span></span>

<span data-ttu-id="99730-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99730-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99730-p102">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="99730-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="99730-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99730-108">Permissions</span></span>
<span data-ttu-id="99730-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99730-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99730-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99730-111">Permission type</span></span>      | <span data-ttu-id="99730-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99730-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99730-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99730-113">Delegated (work or school account)</span></span> | <span data-ttu-id="99730-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99730-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99730-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99730-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99730-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99730-116">Not supported.</span></span>    |
|<span data-ttu-id="99730-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99730-117">Application</span></span> | <span data-ttu-id="99730-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99730-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99730-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99730-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="99730-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99730-120">Request headers</span></span>
| <span data-ttu-id="99730-121">Имя</span><span class="sxs-lookup"><span data-stu-id="99730-121">Name</span></span>       | <span data-ttu-id="99730-122">Описание</span><span class="sxs-lookup"><span data-stu-id="99730-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99730-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99730-123">Authorization</span></span>  | <span data-ttu-id="99730-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99730-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99730-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99730-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="99730-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="99730-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99730-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99730-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="99730-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="99730-130">Response</span></span>

<span data-ttu-id="99730-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99730-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99730-132">Пример</span><span class="sxs-lookup"><span data-stu-id="99730-132">Example</span></span>
<span data-ttu-id="99730-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="99730-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99730-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="99730-134">Request</span></span>
<span data-ttu-id="99730-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99730-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99730-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="99730-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="c"></a>[<span data-ttu-id="99730-137">C#</span><span class="sxs-lookup"><span data-stu-id="99730-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99730-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99730-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99730-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99730-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99730-140">Java</span><span class="sxs-lookup"><span data-stu-id="99730-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99730-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="99730-141">Response</span></span>
<span data-ttu-id="99730-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="99730-142">Here is an example of the response.</span></span> <span data-ttu-id="99730-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="99730-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

