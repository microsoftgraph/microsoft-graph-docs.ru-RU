---
title: 'RangeBorderCollection: ItemAt'
description: Возвращает объект границы, указанный по индексу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0e08bde28f5044c733d0ec4f0c0d6cd05fbd524d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045686"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="0d4bb-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="0d4bb-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="0d4bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d4bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d4bb-105">Возвращает объект границы, указанный по индексу.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-105">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="0d4bb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d4bb-106">Permissions</span></span>
<span data-ttu-id="0d4bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d4bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d4bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d4bb-109">Permission type</span></span>      | <span data-ttu-id="0d4bb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d4bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d4bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d4bb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d4bb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d4bb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0d4bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d4bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d4bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-114">Not supported.</span></span>    |
|<span data-ttu-id="0d4bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d4bb-115">Application</span></span> | <span data-ttu-id="0d4bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d4bb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d4bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="0d4bb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d4bb-118">Request headers</span></span>
| <span data-ttu-id="0d4bb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0d4bb-119">Name</span></span>       | <span data-ttu-id="0d4bb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0d4bb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d4bb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d4bb-121">Authorization</span></span>  | <span data-ttu-id="0d4bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d4bb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0d4bb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0d4bb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d4bb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d4bb-127">Request body</span></span>
<span data-ttu-id="0d4bb-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0d4bb-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="0d4bb-129">Parameter</span></span>    | <span data-ttu-id="0d4bb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4bb-130">Type</span></span>   |<span data-ttu-id="0d4bb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d4bb-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d4bb-132">index</span><span class="sxs-lookup"><span data-stu-id="0d4bb-132">index</span></span>|<span data-ttu-id="0d4bb-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0d4bb-133">Int32</span></span>|<span data-ttu-id="0d4bb-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="0d4bb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4bb-136">Response</span></span>

<span data-ttu-id="0d4bb-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукранжебордер](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-137">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d4bb-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0d4bb-138">Example</span></span>
<span data-ttu-id="0d4bb-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0d4bb-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d4bb-140">Request</span></span>
<span data-ttu-id="0d4bb-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d4bb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d4bb-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```
# <a name="javascript"></a>[<span data-ttu-id="0d4bb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d4bb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangebordercollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d4bb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d4bb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangebordercollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0d4bb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4bb-145">Response</span></span>
<span data-ttu-id="0d4bb-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d4bb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

