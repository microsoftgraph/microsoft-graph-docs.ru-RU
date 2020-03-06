---
title: 'ChartPointsCollection: ItemAt'
description: Получение точки на основании сведений о ее позиции в ряду.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4cb63a9ed8db460a62f1c3783ef534980d322aff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518380"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="6cb7e-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="6cb7e-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="6cb7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cb7e-105">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-105">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="6cb7e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cb7e-106">Permissions</span></span>
<span data-ttu-id="6cb7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb7e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cb7e-109">Permission type</span></span>      | <span data-ttu-id="6cb7e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cb7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cb7e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cb7e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6cb7e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cb7e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6cb7e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cb7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb7e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-114">Not supported.</span></span>    |
|<span data-ttu-id="6cb7e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cb7e-115">Application</span></span> | <span data-ttu-id="6cb7e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cb7e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cb7e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="6cb7e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cb7e-118">Request headers</span></span>
| <span data-ttu-id="6cb7e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6cb7e-119">Name</span></span>       | <span data-ttu-id="6cb7e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6cb7e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6cb7e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cb7e-121">Authorization</span></span>  | <span data-ttu-id="6cb7e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cb7e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6cb7e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6cb7e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb7e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cb7e-127">Request body</span></span>
<span data-ttu-id="6cb7e-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cb7e-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="6cb7e-129">Parameter</span></span>    | <span data-ttu-id="6cb7e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6cb7e-130">Type</span></span>   |<span data-ttu-id="6cb7e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6cb7e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cb7e-132">index</span><span class="sxs-lookup"><span data-stu-id="6cb7e-132">index</span></span>|<span data-ttu-id="6cb7e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb7e-133">Int32</span></span>|<span data-ttu-id="6cb7e-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="6cb7e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cb7e-136">Response</span></span>

<span data-ttu-id="6cb7e-137">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукчартпоинт](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-137">If successful, this method returns `200 OK` response code and [WorkbookChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cb7e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6cb7e-138">Example</span></span>
<span data-ttu-id="6cb7e-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6cb7e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cb7e-140">Request</span></span>
<span data-ttu-id="6cb7e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6cb7e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb7e-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="6cb7e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cb7e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cb7e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cb7e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartpointscollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6cb7e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cb7e-145">Response</span></span>
<span data-ttu-id="6cb7e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cb7e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
