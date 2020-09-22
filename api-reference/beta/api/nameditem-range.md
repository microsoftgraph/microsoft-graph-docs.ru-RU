---
title: 'NamedItem: Range'
description: Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: b3482578d077a5bd75be52c754999b6cde112a52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062385"
---
# <a name="nameditem-range"></a><span data-ttu-id="17fdd-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="17fdd-104">NamedItem: Range</span></span>

<span data-ttu-id="17fdd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17fdd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17fdd-p102">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="17fdd-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="17fdd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17fdd-108">Permissions</span></span>
<span data-ttu-id="17fdd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17fdd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17fdd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17fdd-111">Permission type</span></span>      | <span data-ttu-id="17fdd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17fdd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17fdd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17fdd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="17fdd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17fdd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="17fdd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17fdd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17fdd-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17fdd-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="17fdd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17fdd-117">Application</span></span> | <span data-ttu-id="17fdd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17fdd-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17fdd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17fdd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="17fdd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17fdd-120">Request headers</span></span>
| <span data-ttu-id="17fdd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="17fdd-121">Name</span></span>       | <span data-ttu-id="17fdd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="17fdd-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="17fdd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17fdd-123">Authorization</span></span>  | <span data-ttu-id="17fdd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17fdd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17fdd-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="17fdd-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="17fdd-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="17fdd-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17fdd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17fdd-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="17fdd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="17fdd-130">Response</span></span>

<span data-ttu-id="17fdd-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="17fdd-131">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17fdd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="17fdd-132">Example</span></span>
<span data-ttu-id="17fdd-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="17fdd-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="17fdd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="17fdd-134">Request</span></span>
<span data-ttu-id="17fdd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17fdd-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17fdd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="17fdd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/Range
```
# <a name="c"></a>[<span data-ttu-id="17fdd-137">C#</span><span class="sxs-lookup"><span data-stu-id="17fdd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17fdd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17fdd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17fdd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17fdd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="17fdd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="17fdd-140">Response</span></span>
<span data-ttu-id="17fdd-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17fdd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


