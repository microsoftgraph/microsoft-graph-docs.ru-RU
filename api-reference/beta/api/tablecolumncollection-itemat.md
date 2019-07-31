---
title: 'TableColumnCollection: ItemAt'
description: Возвращает столбец на основании его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fed8fc0ba8c89379b38358c9366bcedad449c848
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990962"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="414b0-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="414b0-103">TableColumnCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="414b0-104">Возвращает столбец на основании его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="414b0-104">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="414b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="414b0-105">Permissions</span></span>
<span data-ttu-id="414b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="414b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="414b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="414b0-108">Permission type</span></span>      | <span data-ttu-id="414b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="414b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="414b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="414b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="414b0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="414b0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="414b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="414b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="414b0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="414b0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="414b0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="414b0-114">Application</span></span> | <span data-ttu-id="414b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="414b0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="414b0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="414b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="414b0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="414b0-117">Request headers</span></span>
| <span data-ttu-id="414b0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="414b0-118">Name</span></span>       | <span data-ttu-id="414b0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="414b0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="414b0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="414b0-120">Authorization</span></span>  | <span data-ttu-id="414b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="414b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="414b0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="414b0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="414b0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="414b0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="414b0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="414b0-126">Request body</span></span>
<span data-ttu-id="414b0-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="414b0-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="414b0-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="414b0-128">Parameter</span></span>    | <span data-ttu-id="414b0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="414b0-129">Type</span></span>   |<span data-ttu-id="414b0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="414b0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="414b0-131">index</span><span class="sxs-lookup"><span data-stu-id="414b0-131">index</span></span>|<span data-ttu-id="414b0-132">number</span><span class="sxs-lookup"><span data-stu-id="414b0-132">number</span></span>|<span data-ttu-id="414b0-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="414b0-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="414b0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="414b0-135">Response</span></span>

<span data-ttu-id="414b0-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="414b0-136">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="414b0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="414b0-137">Example</span></span>
<span data-ttu-id="414b0-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="414b0-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="414b0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="414b0-139">Request</span></span>
<span data-ttu-id="414b0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="414b0-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="414b0-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="414b0-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="414b0-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="414b0-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="414b0-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="414b0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="414b0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="414b0-144">Response</span></span>
<span data-ttu-id="414b0-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="414b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
