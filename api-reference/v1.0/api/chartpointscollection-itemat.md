---
title: 'ChartPointsCollection: ItemAt'
description: Получение точки на основании сведений о ее позиции в ряду.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 91537f67a050d17484c7425eff342049df205df0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937980"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="8ec9d-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="8ec9d-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="8ec9d-104">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-104">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ec9d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec9d-105">Permissions</span></span>
<span data-ttu-id="8ec9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec9d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec9d-108">Permission type</span></span>      | <span data-ttu-id="8ec9d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ec9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ec9d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ec9d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ec9d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ec9d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ec9d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ec9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ec9d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-113">Not supported.</span></span>    |
|<span data-ttu-id="8ec9d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ec9d-114">Application</span></span> | <span data-ttu-id="8ec9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ec9d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ec9d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="8ec9d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ec9d-117">Request headers</span></span>
| <span data-ttu-id="8ec9d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8ec9d-118">Name</span></span>       | <span data-ttu-id="8ec9d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8ec9d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ec9d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ec9d-120">Authorization</span></span>  | <span data-ttu-id="8ec9d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ec9d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ec9d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ec9d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ec9d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ec9d-126">Request body</span></span>
<span data-ttu-id="8ec9d-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ec9d-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="8ec9d-128">Parameter</span></span>    | <span data-ttu-id="8ec9d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8ec9d-129">Type</span></span>   |<span data-ttu-id="8ec9d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8ec9d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ec9d-131">index</span><span class="sxs-lookup"><span data-stu-id="8ec9d-131">index</span></span>|<span data-ttu-id="8ec9d-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec9d-132">Int32</span></span>|<span data-ttu-id="8ec9d-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="8ec9d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ec9d-135">Response</span></span>

<span data-ttu-id="8ec9d-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookChartPoint](../resources/chartpoint.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-136">If successful, this method returns `200 OK` response code and [WorkbookChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ec9d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="8ec9d-137">Example</span></span>
<span data-ttu-id="8ec9d-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8ec9d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ec9d-139">Request</span></span>
<span data-ttu-id="8ec9d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8ec9d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ec9d-141">Response</span></span>
<span data-ttu-id="8ec9d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8ec9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
