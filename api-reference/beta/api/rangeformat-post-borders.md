---
title: Создание объекта RangeBorder
description: С помощью этого API можно создать объект RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1c9d7eb22a11710b41d64c3284e4fd72789d8e4b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577361"
---
# <a name="create-rangeborder"></a><span data-ttu-id="dc097-103">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="dc097-103">Create RangeBorder</span></span>

<span data-ttu-id="dc097-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc097-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc097-105">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="dc097-105">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc097-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc097-106">Permissions</span></span>
<span data-ttu-id="dc097-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc097-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc097-109">Permission type</span></span>      | <span data-ttu-id="dc097-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc097-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc097-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc097-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc097-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc097-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc097-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc097-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc097-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc097-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc097-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc097-115">Application</span></span> | <span data-ttu-id="dc097-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc097-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc097-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc097-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="dc097-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc097-118">Request headers</span></span>
| <span data-ttu-id="dc097-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dc097-119">Name</span></span>       | <span data-ttu-id="dc097-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dc097-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc097-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc097-121">Authorization</span></span>  | <span data-ttu-id="dc097-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc097-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc097-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc097-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc097-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc097-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc097-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc097-127">Request body</span></span>
<span data-ttu-id="dc097-128">В теле запроса поставляем представление JSON объекта [workbookRangeBorder.](../resources/workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="dc097-128">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dc097-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc097-129">Response</span></span>

<span data-ttu-id="dc097-130">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [workbookRangeBorder](../resources/workbookrangeborder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dc097-130">If successful, this method returns `201 Created` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc097-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dc097-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc097-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc097-132">Request</span></span>
<span data-ttu-id="dc097-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc097-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc097-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc097-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
# <a name="c"></a>[<span data-ttu-id="dc097-135">C#</span><span class="sxs-lookup"><span data-stu-id="dc097-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc097-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc097-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc097-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc097-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc097-138">Java</span><span class="sxs-lookup"><span data-stu-id="dc097-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rangeborder-from-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dc097-139">В теле запроса поставляем представление JSON объекта [workbookRangeBorder.](../resources/workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="dc097-139">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dc097-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc097-140">Response</span></span>
<span data-ttu-id="dc097-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc097-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


