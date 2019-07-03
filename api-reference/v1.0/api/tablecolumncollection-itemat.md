---
title: 'TableColumnCollection: ItemAt'
description: Возвращает столбец на основании его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2238f2d685508ffd2d1242edfd36c9c8b16af8dc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447350"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="7c198-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="7c198-103">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="7c198-104">Возвращает столбец на основании его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="7c198-104">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c198-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c198-105">Permissions</span></span>
<span data-ttu-id="7c198-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c198-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c198-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c198-108">Permission type</span></span>      | <span data-ttu-id="7c198-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c198-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c198-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c198-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c198-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c198-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c198-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c198-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c198-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c198-113">Not supported.</span></span>    |
|<span data-ttu-id="7c198-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c198-114">Application</span></span> | <span data-ttu-id="7c198-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c198-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c198-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c198-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7c198-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c198-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="7c198-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c198-118">Request headers</span></span>
| <span data-ttu-id="7c198-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7c198-119">Name</span></span>       | <span data-ttu-id="7c198-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7c198-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c198-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c198-121">Authorization</span></span>  | <span data-ttu-id="7c198-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c198-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c198-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c198-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c198-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7c198-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c198-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c198-127">Request body</span></span>
<span data-ttu-id="7c198-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7c198-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7c198-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="7c198-129">Parameter</span></span>    | <span data-ttu-id="7c198-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c198-130">Type</span></span>   |<span data-ttu-id="7c198-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c198-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c198-132">index</span><span class="sxs-lookup"><span data-stu-id="7c198-132">index</span></span>|<span data-ttu-id="7c198-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7c198-133">Int32</span></span>|<span data-ttu-id="7c198-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="7c198-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7c198-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c198-136">Response</span></span>

<span data-ttu-id="7c198-137">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктаблеколумн](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c198-137">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c198-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7c198-138">Example</span></span>
<span data-ttu-id="7c198-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7c198-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c198-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c198-140">Request</span></span>
<span data-ttu-id="7c198-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c198-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumncollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 3
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c198-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c198-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c198-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7c198-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7c198-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c198-144">Response</span></span>
<span data-ttu-id="7c198-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c198-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
