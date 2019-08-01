---
title: Создание объекта RangeBorder
description: С помощью этого API можно создать объект RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 42a9a1f460dcee68c7ca5b8c445e45f20cc528c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025185"
---
# <a name="create-rangeborder"></a><span data-ttu-id="59720-103">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="59720-103">Create RangeBorder</span></span>

<span data-ttu-id="59720-104">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="59720-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="59720-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59720-105">Permissions</span></span>
<span data-ttu-id="59720-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59720-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59720-108">Permission type</span></span>      | <span data-ttu-id="59720-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59720-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59720-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59720-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59720-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59720-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59720-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59720-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59720-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59720-113">Not supported.</span></span>    |
|<span data-ttu-id="59720-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59720-114">Application</span></span> | <span data-ttu-id="59720-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59720-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59720-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59720-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="59720-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59720-117">Request headers</span></span>
| <span data-ttu-id="59720-118">Имя</span><span class="sxs-lookup"><span data-stu-id="59720-118">Name</span></span>       | <span data-ttu-id="59720-119">Описание</span><span class="sxs-lookup"><span data-stu-id="59720-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59720-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59720-120">Authorization</span></span>  | <span data-ttu-id="59720-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59720-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59720-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59720-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="59720-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="59720-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59720-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59720-126">Request body</span></span>
<span data-ttu-id="59720-127">В тексте запроса добавьте представление объекта [воркбукранжебордер](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59720-127">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="59720-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="59720-128">Response</span></span>

<span data-ttu-id="59720-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбукранжебордер](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59720-129">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59720-130">Пример</span><span class="sxs-lookup"><span data-stu-id="59720-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59720-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="59720-131">Request</span></span>
<span data-ttu-id="59720-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59720-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59720-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="59720-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59720-134">C#</span><span class="sxs-lookup"><span data-stu-id="59720-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59720-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="59720-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59720-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="59720-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59720-137">Java</span><span class="sxs-lookup"><span data-stu-id="59720-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rangeborder-from-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="59720-138">В тексте запроса добавьте представление объекта [воркбукранжебордер](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59720-138">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="59720-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="59720-139">Response</span></span>
<span data-ttu-id="59720-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59720-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
