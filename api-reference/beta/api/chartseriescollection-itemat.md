---
title: 'ChartSeriesCollection: ItemAt'
description: Возвращает ряд на основании сведений о его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 063a5a605908693e5b189c92865eaec2c0dba1ba
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640254"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="bc0ef-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="bc0ef-103">ChartSeriesCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc0ef-104">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="bc0ef-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc0ef-105">Permissions</span></span>
<span data-ttu-id="bc0ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc0ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc0ef-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc0ef-108">Permission type</span></span>      | <span data-ttu-id="bc0ef-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc0ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc0ef-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc0ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc0ef-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc0ef-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc0ef-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc0ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc0ef-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc0ef-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc0ef-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc0ef-114">Application</span></span> | <span data-ttu-id="bc0ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc0ef-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc0ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="bc0ef-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc0ef-117">Request headers</span></span>
| <span data-ttu-id="bc0ef-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bc0ef-118">Name</span></span>       | <span data-ttu-id="bc0ef-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bc0ef-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc0ef-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc0ef-120">Authorization</span></span>  | <span data-ttu-id="bc0ef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc0ef-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc0ef-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc0ef-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc0ef-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc0ef-126">Request body</span></span>
<span data-ttu-id="bc0ef-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bc0ef-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="bc0ef-128">Parameter</span></span>    | <span data-ttu-id="bc0ef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bc0ef-129">Type</span></span>   |<span data-ttu-id="bc0ef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bc0ef-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc0ef-131">index</span><span class="sxs-lookup"><span data-stu-id="bc0ef-131">index</span></span>|<span data-ttu-id="bc0ef-132">число</span><span class="sxs-lookup"><span data-stu-id="bc0ef-132">number</span></span>|<span data-ttu-id="bc0ef-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="bc0ef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc0ef-135">Response</span></span>

<span data-ttu-id="bc0ef-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-136">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc0ef-137">Пример</span><span class="sxs-lookup"><span data-stu-id="bc0ef-137">Example</span></span>
<span data-ttu-id="bc0ef-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bc0ef-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc0ef-139">Request</span></span>
<span data-ttu-id="bc0ef-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="bc0ef-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc0ef-141">Response</span></span>
<span data-ttu-id="bc0ef-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc0ef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
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
    "Error: /api-reference/beta/api/chartseriescollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
