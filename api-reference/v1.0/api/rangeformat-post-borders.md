---
title: Создание объекта RangeBorder
description: С помощью этого API можно создать объект RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c2b3948ed50dd7b5a84e5439860f41549b1195ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510475"
---
# <a name="create-rangeborder"></a><span data-ttu-id="4cdd1-103">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="4cdd1-103">Create RangeBorder</span></span>

<span data-ttu-id="4cdd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cdd1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cdd1-105">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-105">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cdd1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cdd1-106">Permissions</span></span>
<span data-ttu-id="4cdd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cdd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cdd1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cdd1-109">Permission type</span></span>      | <span data-ttu-id="4cdd1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cdd1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cdd1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cdd1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4cdd1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cdd1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4cdd1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cdd1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cdd1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-114">Not supported.</span></span>    |
|<span data-ttu-id="4cdd1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cdd1-115">Application</span></span> | <span data-ttu-id="4cdd1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cdd1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cdd1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="4cdd1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cdd1-118">Request headers</span></span>
| <span data-ttu-id="4cdd1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4cdd1-119">Name</span></span>       | <span data-ttu-id="4cdd1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4cdd1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4cdd1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cdd1-121">Authorization</span></span>  | <span data-ttu-id="4cdd1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cdd1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4cdd1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4cdd1-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cdd1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cdd1-127">Request body</span></span>
<span data-ttu-id="4cdd1-128">В тексте запроса добавьте представление объекта [воркбукранжебордер](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-128">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4cdd1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cdd1-129">Response</span></span>

<span data-ttu-id="4cdd1-130">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбукранжебордер](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-130">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cdd1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4cdd1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cdd1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cdd1-132">Request</span></span>
<span data-ttu-id="4cdd1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4cdd1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cdd1-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4cdd1-135">C#</span><span class="sxs-lookup"><span data-stu-id="4cdd1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cdd1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cdd1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cdd1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cdd1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4cdd1-138">Java</span><span class="sxs-lookup"><span data-stu-id="4cdd1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rangeborder-from-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4cdd1-139">В тексте запроса добавьте представление объекта [воркбукранжебордер](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-139">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4cdd1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cdd1-140">Response</span></span>
<span data-ttu-id="4cdd1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cdd1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
