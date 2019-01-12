---
title: Тип ресурса ChartGridlines
description: Представляет основные или вспомогательные линии сетки на оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 044af64a6b6d41d9d5407678d1bd1e49cbdffe8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928152"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="c2a68-103">Тип ресурса ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c2a68-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="c2a68-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2a68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2a68-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2a68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2a68-106">Представляет основные или вспомогательные линии сетки на оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c2a68-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="c2a68-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c2a68-107">Methods</span></span>

| <span data-ttu-id="c2a68-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c2a68-108">Method</span></span>           | <span data-ttu-id="c2a68-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2a68-109">Return Type</span></span>    |<span data-ttu-id="c2a68-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2a68-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2a68-111">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c2a68-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="c2a68-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c2a68-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="c2a68-113">Чтение свойств и связей объекта chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="c2a68-113">Read properties and relationships of chartGridlines object.</span></span>|
|<span data-ttu-id="c2a68-114">[обновление](../api/chartgridlines-update.md).</span><span class="sxs-lookup"><span data-stu-id="c2a68-114">[Update](../api/chartgridlines-update.md)</span></span> | [<span data-ttu-id="c2a68-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c2a68-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="c2a68-116">Обновление объекта ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="c2a68-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c2a68-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2a68-117">Properties</span></span>
| <span data-ttu-id="c2a68-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2a68-118">Property</span></span>     | <span data-ttu-id="c2a68-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c2a68-119">Type</span></span>   |<span data-ttu-id="c2a68-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c2a68-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2a68-121">visible</span><span class="sxs-lookup"><span data-stu-id="c2a68-121">visible</span></span>|<span data-ttu-id="c2a68-122">boolean</span><span class="sxs-lookup"><span data-stu-id="c2a68-122">boolean</span></span>|<span data-ttu-id="c2a68-123">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="c2a68-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2a68-124">Связи</span><span class="sxs-lookup"><span data-stu-id="c2a68-124">Relationships</span></span>
| <span data-ttu-id="c2a68-125">Связь</span><span class="sxs-lookup"><span data-stu-id="c2a68-125">Relationship</span></span> | <span data-ttu-id="c2a68-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c2a68-126">Type</span></span>   |<span data-ttu-id="c2a68-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c2a68-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2a68-128">format</span><span class="sxs-lookup"><span data-stu-id="c2a68-128">format</span></span>|[<span data-ttu-id="c2a68-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="c2a68-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="c2a68-p102">Представляет форматирование линий сетки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2a68-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2a68-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2a68-132">JSON representation</span></span>

<span data-ttu-id="c2a68-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2a68-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
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
