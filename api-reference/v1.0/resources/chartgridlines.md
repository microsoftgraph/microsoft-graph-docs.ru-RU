---
title: Тип ресурса ChartGridlines
description: Представляет основные или вспомогательные линии сетки на оси диаграммы.
ms.openlocfilehash: 352f2ff93b899a5321787a0f44b75188e671de27
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025260"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="915cd-103">Тип ресурса ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="915cd-103">ChartGridlines resource type</span></span>

<span data-ttu-id="915cd-104">Представляет основные или вспомогательные линии сетки на оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="915cd-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="915cd-105">Методы</span><span class="sxs-lookup"><span data-stu-id="915cd-105">Methods</span></span>

| <span data-ttu-id="915cd-106">Метод</span><span class="sxs-lookup"><span data-stu-id="915cd-106">Method</span></span>           | <span data-ttu-id="915cd-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="915cd-107">Return Type</span></span>    |<span data-ttu-id="915cd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="915cd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="915cd-109">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="915cd-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="915cd-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="915cd-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="915cd-111">Чтение свойств и связей объекта chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="915cd-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="915cd-112">Update</span><span class="sxs-lookup"><span data-stu-id="915cd-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="915cd-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="915cd-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="915cd-114">Обновление объекта ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="915cd-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="915cd-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="915cd-115">Properties</span></span>
| <span data-ttu-id="915cd-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="915cd-116">Property</span></span>     | <span data-ttu-id="915cd-117">Тип</span><span class="sxs-lookup"><span data-stu-id="915cd-117">Type</span></span>   |<span data-ttu-id="915cd-118">Описание</span><span class="sxs-lookup"><span data-stu-id="915cd-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="915cd-119">visible</span><span class="sxs-lookup"><span data-stu-id="915cd-119">visible</span></span>|<span data-ttu-id="915cd-120">boolean</span><span class="sxs-lookup"><span data-stu-id="915cd-120">boolean</span></span>|<span data-ttu-id="915cd-121">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="915cd-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="915cd-122">Связи</span><span class="sxs-lookup"><span data-stu-id="915cd-122">Relationships</span></span>
| <span data-ttu-id="915cd-123">Связь</span><span class="sxs-lookup"><span data-stu-id="915cd-123">Relationship</span></span> | <span data-ttu-id="915cd-124">Тип</span><span class="sxs-lookup"><span data-stu-id="915cd-124">Type</span></span>   |<span data-ttu-id="915cd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="915cd-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="915cd-126">format</span><span class="sxs-lookup"><span data-stu-id="915cd-126">format</span></span>|[<span data-ttu-id="915cd-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="915cd-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="915cd-p101">Представляет форматирование линий сетки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="915cd-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="915cd-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="915cd-130">JSON representation</span></span>

<span data-ttu-id="915cd-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="915cd-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->