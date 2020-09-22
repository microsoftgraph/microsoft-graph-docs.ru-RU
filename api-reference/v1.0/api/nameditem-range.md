---
title: 'NamedItem: Range'
description: Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8dcedaca340f87eae9ecd9dac0a242046bb6dbbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971064"
---
# <a name="nameditem-range"></a><span data-ttu-id="0fd5b-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="0fd5b-104">NamedItem: Range</span></span>

<span data-ttu-id="0fd5b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fd5b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fd5b-p102">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="0fd5b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fd5b-108">Permissions</span></span>
<span data-ttu-id="0fd5b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fd5b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fd5b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fd5b-111">Permission type</span></span>      | <span data-ttu-id="0fd5b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fd5b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fd5b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fd5b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0fd5b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fd5b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0fd5b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fd5b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fd5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-116">Not supported.</span></span>    |
|<span data-ttu-id="0fd5b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fd5b-117">Application</span></span> | <span data-ttu-id="0fd5b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fd5b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fd5b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="0fd5b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fd5b-120">Request headers</span></span>
| <span data-ttu-id="0fd5b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0fd5b-121">Name</span></span>       | <span data-ttu-id="0fd5b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd5b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0fd5b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fd5b-123">Authorization</span></span>  | <span data-ttu-id="0fd5b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0fd5b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0fd5b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="0fd5b-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fd5b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fd5b-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0fd5b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fd5b-130">Response</span></span>

<span data-ttu-id="0fd5b-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fd5b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0fd5b-132">Example</span></span>
<span data-ttu-id="0fd5b-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0fd5b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fd5b-134">Request</span></span>
<span data-ttu-id="0fd5b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fd5b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fd5b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="c"></a>[<span data-ttu-id="0fd5b-137">C#</span><span class="sxs-lookup"><span data-stu-id="0fd5b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fd5b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fd5b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fd5b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fd5b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fd5b-140">Java</span><span class="sxs-lookup"><span data-stu-id="0fd5b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0fd5b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fd5b-141">Response</span></span>
<span data-ttu-id="0fd5b-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fd5b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

