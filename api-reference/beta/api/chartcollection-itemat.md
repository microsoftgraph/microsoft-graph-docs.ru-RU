---
title: 'ChartCollection: ItemAt'
description: Возвращает диаграмму на основании сведений о ее позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 82e5d79ee4498a5b5b4e2fc2adc0461aec13cae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521714"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="13cdd-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="13cdd-103">ChartCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13cdd-104">Возвращает диаграмму на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="13cdd-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="13cdd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13cdd-105">Permissions</span></span>
<span data-ttu-id="13cdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13cdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13cdd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13cdd-108">Permission type</span></span>      | <span data-ttu-id="13cdd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13cdd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13cdd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13cdd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13cdd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13cdd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13cdd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13cdd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13cdd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13cdd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13cdd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13cdd-114">Application</span></span> | <span data-ttu-id="13cdd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13cdd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13cdd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13cdd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="13cdd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13cdd-117">Request headers</span></span>
| <span data-ttu-id="13cdd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="13cdd-118">Name</span></span>       | <span data-ttu-id="13cdd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="13cdd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="13cdd-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13cdd-120">Authorization</span></span>  | <span data-ttu-id="13cdd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13cdd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13cdd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="13cdd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="13cdd-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="13cdd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13cdd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13cdd-126">Request body</span></span>
<span data-ttu-id="13cdd-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="13cdd-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="13cdd-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="13cdd-128">Parameter</span></span>    | <span data-ttu-id="13cdd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="13cdd-129">Type</span></span>   |<span data-ttu-id="13cdd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="13cdd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13cdd-131">index</span><span class="sxs-lookup"><span data-stu-id="13cdd-131">index</span></span>|<span data-ttu-id="13cdd-132">число</span><span class="sxs-lookup"><span data-stu-id="13cdd-132">number</span></span>|<span data-ttu-id="13cdd-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="13cdd-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="13cdd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cdd-135">Response</span></span>

<span data-ttu-id="13cdd-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13cdd-136">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13cdd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="13cdd-137">Example</span></span>
<span data-ttu-id="13cdd-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="13cdd-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="13cdd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="13cdd-139">Request</span></span>
<span data-ttu-id="13cdd-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13cdd-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="13cdd-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="13cdd-141">Response</span></span>
<span data-ttu-id="13cdd-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="13cdd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
