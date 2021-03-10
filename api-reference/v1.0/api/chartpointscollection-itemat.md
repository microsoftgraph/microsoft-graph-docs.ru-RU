---
title: 'ChartPointsCollection: ItemAt'
description: Получение точки на основании сведений о ее позиции в ряду.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 300a561113abdae978531f080fe8ac8b2fb1f638
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575590"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="4a11c-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="4a11c-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="4a11c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a11c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a11c-105">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="4a11c-105">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a11c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a11c-106">Permissions</span></span>
<span data-ttu-id="4a11c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a11c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a11c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a11c-109">Permission type</span></span>      | <span data-ttu-id="4a11c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a11c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a11c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a11c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a11c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a11c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a11c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a11c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a11c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a11c-114">Not supported.</span></span>    |
|<span data-ttu-id="4a11c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a11c-115">Application</span></span> | <span data-ttu-id="4a11c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a11c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a11c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a11c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="4a11c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a11c-118">Request headers</span></span>
| <span data-ttu-id="4a11c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a11c-119">Name</span></span>       | <span data-ttu-id="4a11c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a11c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a11c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a11c-121">Authorization</span></span>  | <span data-ttu-id="4a11c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a11c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a11c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4a11c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a11c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4a11c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a11c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a11c-127">Request body</span></span>
<span data-ttu-id="4a11c-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4a11c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a11c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a11c-129">Parameter</span></span>    | <span data-ttu-id="4a11c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4a11c-130">Type</span></span>   |<span data-ttu-id="4a11c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4a11c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a11c-132">index</span><span class="sxs-lookup"><span data-stu-id="4a11c-132">index</span></span>|<span data-ttu-id="4a11c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="4a11c-133">Int32</span></span>|<span data-ttu-id="4a11c-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="4a11c-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="4a11c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a11c-136">Response</span></span>

<span data-ttu-id="4a11c-137">В случае успеха этот метод возвращает код ответа и `200 OK` [объект WorkbookChartPoint](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a11c-137">If successful, this method returns `200 OK` response code and [WorkbookChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a11c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4a11c-138">Example</span></span>
<span data-ttu-id="4a11c-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4a11c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a11c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a11c-140">Request</span></span>
<span data-ttu-id="4a11c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a11c-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a11c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a11c-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="4a11c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a11c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a11c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a11c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartpointscollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4a11c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a11c-145">Response</span></span>
<span data-ttu-id="4a11c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a11c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

