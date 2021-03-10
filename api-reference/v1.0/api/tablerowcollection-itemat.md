---
title: 'TableRowCollection: ItemAt'
description: Получает строку на основании сведений о ее позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 573dfa8cf923ba5f988c0c8e4fa39b87ac8dd454
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577893"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="e8876-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e8876-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="e8876-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8876-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8876-105">Получает строку на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="e8876-105">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8876-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8876-106">Permissions</span></span>
<span data-ttu-id="e8876-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8876-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8876-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8876-109">Permission type</span></span>      | <span data-ttu-id="e8876-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8876-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8876-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8876-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e8876-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8876-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8876-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8876-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8876-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8876-114">Not supported.</span></span>    |
|<span data-ttu-id="e8876-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8876-115">Application</span></span> | <span data-ttu-id="e8876-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8876-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8876-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8876-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/itemAt
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="e8876-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8876-118">Request headers</span></span>
| <span data-ttu-id="e8876-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e8876-119">Name</span></span>       | <span data-ttu-id="e8876-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8876-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8876-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8876-121">Authorization</span></span>  | <span data-ttu-id="e8876-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8876-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8876-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e8876-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8876-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e8876-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8876-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8876-127">Request body</span></span>
<span data-ttu-id="e8876-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e8876-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e8876-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="e8876-129">Parameter</span></span>    | <span data-ttu-id="e8876-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e8876-130">Type</span></span>   |<span data-ttu-id="e8876-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e8876-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8876-132">index</span><span class="sxs-lookup"><span data-stu-id="e8876-132">index</span></span>|<span data-ttu-id="e8876-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e8876-133">Int32</span></span>|<span data-ttu-id="e8876-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="e8876-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e8876-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8876-136">Response</span></span>

<span data-ttu-id="e8876-137">В случае успеха этот метод возвращает код отклика и `200 OK` [объект WorkbookTableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8876-137">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8876-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e8876-138">Example</span></span>
<span data-ttu-id="e8876-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e8876-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e8876-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8876-140">Request</span></span>
<span data-ttu-id="e8876-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8876-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8876-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8876-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerowcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 4
}
```
# <a name="javascript"></a>[<span data-ttu-id="e8876-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8876-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8876-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8876-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e8876-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8876-145">Response</span></span>
<span data-ttu-id="e8876-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8876-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

