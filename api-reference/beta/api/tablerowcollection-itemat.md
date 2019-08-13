---
title: 'TableRowCollection: ItemAt'
description: Получает строку на основании сведений о ее позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0b8f7d89fbd75ed78dc7d5dfbf375163df3d03ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362950"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="be806-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="be806-103">TableRowCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be806-104">Получает строку на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="be806-104">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="be806-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be806-105">Permissions</span></span>
<span data-ttu-id="be806-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be806-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be806-108">Permission type</span></span>      | <span data-ttu-id="be806-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be806-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be806-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be806-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be806-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be806-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be806-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be806-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be806-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be806-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be806-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be806-114">Application</span></span> | <span data-ttu-id="be806-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be806-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be806-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be806-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="be806-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be806-117">Request headers</span></span>
| <span data-ttu-id="be806-118">Имя</span><span class="sxs-lookup"><span data-stu-id="be806-118">Name</span></span>       | <span data-ttu-id="be806-119">Описание</span><span class="sxs-lookup"><span data-stu-id="be806-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be806-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be806-120">Authorization</span></span>  | <span data-ttu-id="be806-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be806-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be806-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be806-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="be806-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="be806-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be806-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be806-126">Request body</span></span>
<span data-ttu-id="be806-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="be806-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="be806-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="be806-128">Parameter</span></span>    | <span data-ttu-id="be806-129">Тип</span><span class="sxs-lookup"><span data-stu-id="be806-129">Type</span></span>   |<span data-ttu-id="be806-130">Описание</span><span class="sxs-lookup"><span data-stu-id="be806-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be806-131">index</span><span class="sxs-lookup"><span data-stu-id="be806-131">index</span></span>|<span data-ttu-id="be806-132">number</span><span class="sxs-lookup"><span data-stu-id="be806-132">number</span></span>|<span data-ttu-id="be806-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="be806-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="be806-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="be806-135">Response</span></span>

<span data-ttu-id="be806-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктаблеров](../resources/workbooktablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be806-136">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be806-137">Пример</span><span class="sxs-lookup"><span data-stu-id="be806-137">Example</span></span>
<span data-ttu-id="be806-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="be806-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="be806-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="be806-139">Request</span></span>
<span data-ttu-id="be806-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be806-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be806-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="be806-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be806-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be806-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be806-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="be806-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="be806-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="be806-144">Response</span></span>
<span data-ttu-id="be806-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be806-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
