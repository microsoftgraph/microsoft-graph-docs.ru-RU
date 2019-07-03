---
title: 'ChartPointsCollection: ItemAt'
description: Получение точки на основании сведений о ее позиции в ряду.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0904a60381e6a937094d3c856f43423bd4db3283
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437987"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="09c58-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="09c58-103">ChartPointsCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09c58-104">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="09c58-104">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="09c58-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09c58-105">Permissions</span></span>
<span data-ttu-id="09c58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09c58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09c58-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09c58-108">Permission type</span></span>      | <span data-ttu-id="09c58-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09c58-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09c58-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09c58-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09c58-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09c58-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="09c58-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09c58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09c58-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09c58-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="09c58-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09c58-114">Application</span></span> | <span data-ttu-id="09c58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09c58-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09c58-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09c58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="09c58-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09c58-117">Request headers</span></span>
| <span data-ttu-id="09c58-118">Имя</span><span class="sxs-lookup"><span data-stu-id="09c58-118">Name</span></span>       | <span data-ttu-id="09c58-119">Описание</span><span class="sxs-lookup"><span data-stu-id="09c58-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="09c58-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09c58-120">Authorization</span></span>  | <span data-ttu-id="09c58-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09c58-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09c58-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="09c58-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="09c58-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="09c58-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09c58-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09c58-126">Request body</span></span>
<span data-ttu-id="09c58-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="09c58-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09c58-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="09c58-128">Parameter</span></span>    | <span data-ttu-id="09c58-129">Тип</span><span class="sxs-lookup"><span data-stu-id="09c58-129">Type</span></span>   |<span data-ttu-id="09c58-130">Описание</span><span class="sxs-lookup"><span data-stu-id="09c58-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09c58-131">index</span><span class="sxs-lookup"><span data-stu-id="09c58-131">index</span></span>|<span data-ttu-id="09c58-132">number</span><span class="sxs-lookup"><span data-stu-id="09c58-132">number</span></span>|<span data-ttu-id="09c58-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="09c58-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="09c58-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="09c58-135">Response</span></span>

<span data-ttu-id="09c58-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукчартпоинт](../resources/workbookchartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09c58-136">If successful, this method returns `200 OK` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09c58-137">Пример</span><span class="sxs-lookup"><span data-stu-id="09c58-137">Example</span></span>
<span data-ttu-id="09c58-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="09c58-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09c58-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="09c58-139">Request</span></span>
<span data-ttu-id="09c58-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09c58-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="09c58-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="09c58-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09c58-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="09c58-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="09c58-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="09c58-143">Response</span></span>
<span data-ttu-id="09c58-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09c58-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
