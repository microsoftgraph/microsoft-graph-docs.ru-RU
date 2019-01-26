---
title: 'ChartPointsCollection: ItemAt'
description: Получение точки на основании сведений о ее позиции в ряду.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a7a4274790f39bc8443273df0fb617e65a564372
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577209"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="21a01-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="21a01-103">ChartPointsCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21a01-104">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="21a01-104">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="21a01-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21a01-105">Permissions</span></span>
<span data-ttu-id="21a01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21a01-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21a01-108">Permission type</span></span>      | <span data-ttu-id="21a01-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21a01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21a01-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21a01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21a01-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21a01-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21a01-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21a01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21a01-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21a01-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21a01-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21a01-114">Application</span></span> | <span data-ttu-id="21a01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21a01-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21a01-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21a01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="21a01-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21a01-117">Request headers</span></span>
| <span data-ttu-id="21a01-118">Имя</span><span class="sxs-lookup"><span data-stu-id="21a01-118">Name</span></span>       | <span data-ttu-id="21a01-119">Описание</span><span class="sxs-lookup"><span data-stu-id="21a01-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="21a01-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21a01-120">Authorization</span></span>  | <span data-ttu-id="21a01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21a01-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21a01-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="21a01-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="21a01-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="21a01-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21a01-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21a01-126">Request body</span></span>
<span data-ttu-id="21a01-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="21a01-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="21a01-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="21a01-128">Parameter</span></span>    | <span data-ttu-id="21a01-129">Тип</span><span class="sxs-lookup"><span data-stu-id="21a01-129">Type</span></span>   |<span data-ttu-id="21a01-130">Описание</span><span class="sxs-lookup"><span data-stu-id="21a01-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21a01-131">index</span><span class="sxs-lookup"><span data-stu-id="21a01-131">index</span></span>|<span data-ttu-id="21a01-132">число</span><span class="sxs-lookup"><span data-stu-id="21a01-132">number</span></span>|<span data-ttu-id="21a01-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="21a01-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="21a01-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="21a01-135">Response</span></span>

<span data-ttu-id="21a01-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartPoint](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21a01-136">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21a01-137">Пример</span><span class="sxs-lookup"><span data-stu-id="21a01-137">Example</span></span>
<span data-ttu-id="21a01-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="21a01-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="21a01-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="21a01-139">Request</span></span>
<span data-ttu-id="21a01-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21a01-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="21a01-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="21a01-141">Response</span></span>
<span data-ttu-id="21a01-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="21a01-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/chartpointscollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
