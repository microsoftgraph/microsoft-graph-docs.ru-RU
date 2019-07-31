---
title: 'ChartSeriesCollection: ItemAt'
description: Возвращает ряд на основании сведений о его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 09060e1ed79f24afb1b6e3419485dea419d60f37
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943689"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="c4143-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="c4143-103">ChartSeriesCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4143-104">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="c4143-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="c4143-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4143-105">Permissions</span></span>
<span data-ttu-id="c4143-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4143-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4143-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4143-108">Permission type</span></span>      | <span data-ttu-id="c4143-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4143-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4143-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4143-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4143-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4143-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4143-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4143-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4143-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4143-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4143-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4143-114">Application</span></span> | <span data-ttu-id="c4143-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4143-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4143-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4143-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="c4143-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4143-117">Request headers</span></span>
| <span data-ttu-id="c4143-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c4143-118">Name</span></span>       | <span data-ttu-id="c4143-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c4143-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4143-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4143-120">Authorization</span></span>  | <span data-ttu-id="c4143-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4143-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4143-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4143-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4143-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c4143-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4143-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4143-126">Request body</span></span>
<span data-ttu-id="c4143-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c4143-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4143-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4143-128">Parameter</span></span>    | <span data-ttu-id="c4143-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c4143-129">Type</span></span>   |<span data-ttu-id="c4143-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c4143-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4143-131">index</span><span class="sxs-lookup"><span data-stu-id="c4143-131">index</span></span>|<span data-ttu-id="c4143-132">number</span><span class="sxs-lookup"><span data-stu-id="c4143-132">number</span></span>|<span data-ttu-id="c4143-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="c4143-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="c4143-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4143-135">Response</span></span>

<span data-ttu-id="c4143-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукчартсериес](../resources/workbookchartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4143-136">If successful, this method returns `200 OK` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4143-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c4143-137">Example</span></span>
<span data-ttu-id="c4143-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c4143-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4143-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4143-139">Request</span></span>
<span data-ttu-id="c4143-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4143-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c4143-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4143-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4143-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="c4143-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartseriescollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4143-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4143-143">Response</span></span>
<span data-ttu-id="c4143-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4143-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
