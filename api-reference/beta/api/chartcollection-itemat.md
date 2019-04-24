---
title: 'ChartCollection: ItemAt'
description: Возвращает диаграмму на основании сведений о ее позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 82e5d79ee4498a5b5b4e2fc2adc0461aec13cae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456600"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="91cdf-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="91cdf-103">ChartCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91cdf-104">Возвращает диаграмму на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="91cdf-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="91cdf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91cdf-105">Permissions</span></span>
<span data-ttu-id="91cdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91cdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91cdf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91cdf-108">Permission type</span></span>      | <span data-ttu-id="91cdf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91cdf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91cdf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91cdf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91cdf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91cdf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91cdf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91cdf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91cdf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91cdf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91cdf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91cdf-114">Application</span></span> | <span data-ttu-id="91cdf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91cdf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91cdf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91cdf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="91cdf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91cdf-117">Request headers</span></span>
| <span data-ttu-id="91cdf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="91cdf-118">Name</span></span>       | <span data-ttu-id="91cdf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="91cdf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91cdf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91cdf-120">Authorization</span></span>  | <span data-ttu-id="91cdf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91cdf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91cdf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="91cdf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="91cdf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="91cdf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91cdf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91cdf-126">Request body</span></span>
<span data-ttu-id="91cdf-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="91cdf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="91cdf-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="91cdf-128">Parameter</span></span>    | <span data-ttu-id="91cdf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="91cdf-129">Type</span></span>   |<span data-ttu-id="91cdf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="91cdf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91cdf-131">index</span><span class="sxs-lookup"><span data-stu-id="91cdf-131">index</span></span>|<span data-ttu-id="91cdf-132">number</span><span class="sxs-lookup"><span data-stu-id="91cdf-132">number</span></span>|<span data-ttu-id="91cdf-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="91cdf-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="91cdf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="91cdf-135">Response</span></span>

<span data-ttu-id="91cdf-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91cdf-136">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91cdf-137">Пример</span><span class="sxs-lookup"><span data-stu-id="91cdf-137">Example</span></span>
<span data-ttu-id="91cdf-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="91cdf-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91cdf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="91cdf-139">Request</span></span>
<span data-ttu-id="91cdf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91cdf-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="91cdf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="91cdf-141">Response</span></span>
<span data-ttu-id="91cdf-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91cdf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartcollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
