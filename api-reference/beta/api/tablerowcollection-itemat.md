---
title: 'TableRowCollection: ItemAt'
description: Получает строку на основании сведений о ее позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1fcb87a1422b28c8f086dc619076dba6ddd578c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054786"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="e9401-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e9401-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="e9401-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9401-105">Получает строку на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="e9401-105">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9401-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9401-106">Permissions</span></span>
<span data-ttu-id="e9401-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9401-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9401-109">Permission type</span></span>      | <span data-ttu-id="e9401-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9401-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9401-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9401-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9401-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9401-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9401-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9401-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9401-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9401-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9401-115">Application</span></span> | <span data-ttu-id="e9401-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9401-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9401-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9401-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/ItemAt
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="e9401-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9401-118">Request headers</span></span>
| <span data-ttu-id="e9401-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e9401-119">Name</span></span>       | <span data-ttu-id="e9401-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e9401-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e9401-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9401-121">Authorization</span></span>  | <span data-ttu-id="e9401-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9401-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9401-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e9401-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e9401-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e9401-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9401-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9401-127">Request body</span></span>
<span data-ttu-id="e9401-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e9401-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9401-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="e9401-129">Parameter</span></span>    | <span data-ttu-id="e9401-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e9401-130">Type</span></span>   |<span data-ttu-id="e9401-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e9401-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9401-132">index</span><span class="sxs-lookup"><span data-stu-id="e9401-132">index</span></span>|<span data-ttu-id="e9401-133">number</span><span class="sxs-lookup"><span data-stu-id="e9401-133">number</span></span>|<span data-ttu-id="e9401-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="e9401-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e9401-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9401-136">Response</span></span>

<span data-ttu-id="e9401-137">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [workbookTableRow](../resources/workbooktablerow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e9401-137">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9401-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e9401-138">Example</span></span>
<span data-ttu-id="e9401-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e9401-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9401-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9401-140">Request</span></span>
<span data-ttu-id="e9401-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9401-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9401-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9401-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="e9401-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9401-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9401-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9401-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e9401-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9401-145">Response</span></span>
<span data-ttu-id="e9401-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9401-146">Here is an example of the response.</span></span> <span data-ttu-id="e9401-147">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e9401-147">Note: The response object shown here might be shortened for readability.</span></span>
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


