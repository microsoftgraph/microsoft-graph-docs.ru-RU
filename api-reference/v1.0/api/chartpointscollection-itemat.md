---
title: 'ChartPointsCollection: ItemAt'
description: Получение точки на основании сведений о ее позиции в ряду.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 23a74dcd0048716edc46f4f006a083d55f973b89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003408"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="1a1a0-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="1a1a0-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="1a1a0-104">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-104">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a1a0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a1a0-105">Permissions</span></span>
<span data-ttu-id="1a1a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a1a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a1a0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a1a0-108">Permission type</span></span>      | <span data-ttu-id="1a1a0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a1a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a1a0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a1a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a1a0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a1a0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a1a0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a1a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a1a0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-113">Not supported.</span></span>    |
|<span data-ttu-id="1a1a0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a1a0-114">Application</span></span> | <span data-ttu-id="1a1a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a1a0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a1a0-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a1a0-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a1a0-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="1a1a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a1a0-118">Request headers</span></span>
| <span data-ttu-id="1a1a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1a1a0-119">Name</span></span>       | <span data-ttu-id="1a1a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1a1a0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a1a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a1a0-121">Authorization</span></span>  | <span data-ttu-id="1a1a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a1a0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1a1a0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1a1a0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a1a0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a1a0-127">Request body</span></span>
<span data-ttu-id="1a1a0-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a1a0-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="1a1a0-129">Parameter</span></span>    | <span data-ttu-id="1a1a0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a1a0-130">Type</span></span>   |<span data-ttu-id="1a1a0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a1a0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a1a0-132">index</span><span class="sxs-lookup"><span data-stu-id="1a1a0-132">index</span></span>|<span data-ttu-id="1a1a0-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1a1a0-133">Int32</span></span>|<span data-ttu-id="1a1a0-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="1a1a0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a1a0-136">Response</span></span>

<span data-ttu-id="1a1a0-137">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукчартпоинт](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-137">If successful, this method returns `200 OK` response code and [WorkbookChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a1a0-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1a1a0-138">Example</span></span>
<span data-ttu-id="1a1a0-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1a1a0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a1a0-140">Request</span></span>
<span data-ttu-id="1a1a0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartpointscollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a1a0-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a1a0-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a1a0-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1a1a0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartpointscollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1a1a0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a1a0-144">Response</span></span>
<span data-ttu-id="1a1a0-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a1a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
