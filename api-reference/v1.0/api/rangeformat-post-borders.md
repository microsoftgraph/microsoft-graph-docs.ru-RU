---
title: Создание объекта RangeBorder
description: С помощью этого API можно создать объект RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 740db5b32d091c0b0d08fe71e936eb68a477ec33
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023123"
---
# <a name="create-rangeborder"></a><span data-ttu-id="1560a-103">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="1560a-103">Create RangeBorder</span></span>

<span data-ttu-id="1560a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1560a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1560a-105">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="1560a-105">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="1560a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1560a-106">Permissions</span></span>
<span data-ttu-id="1560a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1560a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1560a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1560a-109">Permission type</span></span>      | <span data-ttu-id="1560a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1560a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1560a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1560a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1560a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1560a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1560a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1560a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1560a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1560a-114">Not supported.</span></span>    |
|<span data-ttu-id="1560a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1560a-115">Application</span></span> | <span data-ttu-id="1560a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1560a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1560a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1560a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="1560a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1560a-118">Request headers</span></span>
| <span data-ttu-id="1560a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1560a-119">Name</span></span>       | <span data-ttu-id="1560a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1560a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1560a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1560a-121">Authorization</span></span>  | <span data-ttu-id="1560a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1560a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1560a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1560a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1560a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1560a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1560a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1560a-127">Request body</span></span>
<span data-ttu-id="1560a-128">В тексте запроса добавьте представление объекта [воркбукранжебордер](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1560a-128">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1560a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1560a-129">Response</span></span>

<span data-ttu-id="1560a-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [воркбукранжебордер](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1560a-130">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1560a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1560a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1560a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1560a-132">Request</span></span>
<span data-ttu-id="1560a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1560a-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1560a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1560a-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1560a-135">C#</span><span class="sxs-lookup"><span data-stu-id="1560a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1560a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1560a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1560a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1560a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1560a-138">Java</span><span class="sxs-lookup"><span data-stu-id="1560a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rangeborder-from-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1560a-139">В тексте запроса добавьте представление объекта [воркбукранжебордер](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1560a-139">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1560a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1560a-140">Response</span></span>
<span data-ttu-id="1560a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1560a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

