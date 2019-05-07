---
title: 'TableRowCollection: ItemAt'
description: Получает строку на основании сведений о ее позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8cf67999f3ff67b5463b7b105154679a87b792c6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602437"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="48edf-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="48edf-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="48edf-104">Получает строку на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="48edf-104">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="48edf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48edf-105">Permissions</span></span>
<span data-ttu-id="48edf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48edf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48edf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48edf-108">Permission type</span></span>      | <span data-ttu-id="48edf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48edf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48edf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48edf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48edf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48edf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="48edf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48edf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48edf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48edf-113">Not supported.</span></span>    |
|<span data-ttu-id="48edf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48edf-114">Application</span></span> | <span data-ttu-id="48edf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48edf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48edf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48edf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="48edf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48edf-117">Request headers</span></span>
| <span data-ttu-id="48edf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="48edf-118">Name</span></span>       | <span data-ttu-id="48edf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="48edf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48edf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48edf-120">Authorization</span></span>  | <span data-ttu-id="48edf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48edf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48edf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="48edf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="48edf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="48edf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48edf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48edf-126">Request body</span></span>
<span data-ttu-id="48edf-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="48edf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48edf-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="48edf-128">Parameter</span></span>    | <span data-ttu-id="48edf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="48edf-129">Type</span></span>   |<span data-ttu-id="48edf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="48edf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48edf-131">index</span><span class="sxs-lookup"><span data-stu-id="48edf-131">index</span></span>|<span data-ttu-id="48edf-132">Int32</span><span class="sxs-lookup"><span data-stu-id="48edf-132">Int32</span></span>|<span data-ttu-id="48edf-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="48edf-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="48edf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="48edf-135">Response</span></span>

<span data-ttu-id="48edf-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктаблеров](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48edf-136">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48edf-137">Пример</span><span class="sxs-lookup"><span data-stu-id="48edf-137">Example</span></span>
<span data-ttu-id="48edf-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="48edf-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="48edf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="48edf-139">Request</span></span>
<span data-ttu-id="48edf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48edf-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="48edf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="48edf-141">Response</span></span>
<span data-ttu-id="48edf-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48edf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="48edf-145">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="48edf-145">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48edf-146">Язык</span><span class="sxs-lookup"><span data-stu-id="48edf-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablerowcollection_itemat-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablerowcollection-itemat.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
