---
title: 'TableColumnCollection: ItemAt'
description: Возвращает столбец на основании его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: af3466234df64bd800d06514e9d25a48142374e3
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034058"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="bb159-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="bb159-103">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="bb159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb159-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb159-105">Возвращает столбец на основании его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="bb159-105">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb159-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb159-106">Permissions</span></span>
<span data-ttu-id="bb159-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb159-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb159-109">Permission type</span></span>      | <span data-ttu-id="bb159-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb159-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb159-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb159-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb159-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb159-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb159-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb159-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb159-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb159-114">Not supported.</span></span>    |
|<span data-ttu-id="bb159-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb159-115">Application</span></span> | <span data-ttu-id="bb159-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb159-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb159-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb159-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="bb159-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb159-118">Request headers</span></span>
| <span data-ttu-id="bb159-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bb159-119">Name</span></span>       | <span data-ttu-id="bb159-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bb159-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bb159-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb159-121">Authorization</span></span>  | <span data-ttu-id="bb159-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb159-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb159-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bb159-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="bb159-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bb159-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb159-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb159-127">Request body</span></span>
<span data-ttu-id="bb159-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bb159-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bb159-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb159-129">Parameter</span></span>    | <span data-ttu-id="bb159-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bb159-130">Type</span></span>   |<span data-ttu-id="bb159-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bb159-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb159-132">index</span><span class="sxs-lookup"><span data-stu-id="bb159-132">index</span></span>|<span data-ttu-id="bb159-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bb159-133">Int32</span></span>|<span data-ttu-id="bb159-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="bb159-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="bb159-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb159-136">Response</span></span>

<span data-ttu-id="bb159-137">В случае успеха этот метод возвращает код отклика и объект `200 OK` [WorkbookTableColumn](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb159-137">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb159-138">Пример</span><span class="sxs-lookup"><span data-stu-id="bb159-138">Example</span></span>
<span data-ttu-id="bb159-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bb159-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb159-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb159-140">Request</span></span>
<span data-ttu-id="bb159-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb159-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb159-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb159-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="bb159-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb159-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb159-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb159-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb159-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb159-145">Response</span></span>
<span data-ttu-id="bb159-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb159-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "99",
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

