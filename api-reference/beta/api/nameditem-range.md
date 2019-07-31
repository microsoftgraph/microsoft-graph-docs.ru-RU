---
title: 'NamedItem: Range'
description: Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 823374c03910247ff6fb4ba9af5957a886c496ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992726"
---
# <a name="nameditem-range"></a><span data-ttu-id="d8851-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="d8851-104">NamedItem: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8851-p102">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="d8851-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8851-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8851-107">Permissions</span></span>
<span data-ttu-id="d8851-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8851-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8851-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8851-110">Permission type</span></span>      | <span data-ttu-id="d8851-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8851-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8851-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8851-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8851-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8851-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d8851-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8851-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8851-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8851-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d8851-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8851-116">Application</span></span> | <span data-ttu-id="d8851-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8851-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8851-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8851-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="d8851-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8851-119">Request headers</span></span>
| <span data-ttu-id="d8851-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d8851-120">Name</span></span>       | <span data-ttu-id="d8851-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d8851-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d8851-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8851-122">Authorization</span></span>  | <span data-ttu-id="d8851-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8851-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8851-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d8851-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d8851-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d8851-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8851-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8851-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d8851-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8851-129">Response</span></span>

<span data-ttu-id="d8851-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d8851-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8851-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8851-131">Example</span></span>
<span data-ttu-id="d8851-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d8851-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d8851-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8851-133">Request</span></span>
<span data-ttu-id="d8851-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8851-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8851-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8851-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/Range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8851-136">C#</span><span class="sxs-lookup"><span data-stu-id="d8851-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8851-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8851-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8851-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d8851-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d8851-139">Java</span><span class="sxs-lookup"><span data-stu-id="d8851-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8851-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8851-140">Response</span></span>
<span data-ttu-id="d8851-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8851-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
