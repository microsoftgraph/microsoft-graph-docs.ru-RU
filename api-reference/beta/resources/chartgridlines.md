---
title: Тип ресурса ChartGridlines
description: Представляет основные или вспомогательные линии сетки на оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7747564b2f72287ef6ec2c6cc1f912695f58218e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807828"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="91c86-103">Тип ресурса ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="91c86-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="91c86-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91c86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91c86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91c86-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91c86-106">Представляет основные или вспомогательные линии сетки на оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="91c86-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="91c86-107">Методы</span><span class="sxs-lookup"><span data-stu-id="91c86-107">Methods</span></span>

| <span data-ttu-id="91c86-108">Метод</span><span class="sxs-lookup"><span data-stu-id="91c86-108">Method</span></span>           | <span data-ttu-id="91c86-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="91c86-109">Return Type</span></span>    |<span data-ttu-id="91c86-110">Описание</span><span class="sxs-lookup"><span data-stu-id="91c86-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91c86-111">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="91c86-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="91c86-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="91c86-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="91c86-113">Чтение свойств и связей объекта chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="91c86-113">Read properties and relationships of chartGridlines object.</span></span>|
|<span data-ttu-id="91c86-114">[обновление](../api/chartgridlines-update.md).</span><span class="sxs-lookup"><span data-stu-id="91c86-114">[Update](../api/chartgridlines-update.md)</span></span> | [<span data-ttu-id="91c86-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="91c86-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="91c86-116">Обновление объекта ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="91c86-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="91c86-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="91c86-117">Properties</span></span>
| <span data-ttu-id="91c86-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="91c86-118">Property</span></span>     | <span data-ttu-id="91c86-119">Тип</span><span class="sxs-lookup"><span data-stu-id="91c86-119">Type</span></span>   |<span data-ttu-id="91c86-120">Описание</span><span class="sxs-lookup"><span data-stu-id="91c86-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91c86-121">visible</span><span class="sxs-lookup"><span data-stu-id="91c86-121">visible</span></span>|<span data-ttu-id="91c86-122">boolean</span><span class="sxs-lookup"><span data-stu-id="91c86-122">boolean</span></span>|<span data-ttu-id="91c86-123">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="91c86-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91c86-124">Связи</span><span class="sxs-lookup"><span data-stu-id="91c86-124">Relationships</span></span>
| <span data-ttu-id="91c86-125">Связь</span><span class="sxs-lookup"><span data-stu-id="91c86-125">Relationship</span></span> | <span data-ttu-id="91c86-126">Тип</span><span class="sxs-lookup"><span data-stu-id="91c86-126">Type</span></span>   |<span data-ttu-id="91c86-127">Описание</span><span class="sxs-lookup"><span data-stu-id="91c86-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91c86-128">format</span><span class="sxs-lookup"><span data-stu-id="91c86-128">format</span></span>|[<span data-ttu-id="91c86-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="91c86-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="91c86-p102">Представляет форматирование линий сетки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91c86-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91c86-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91c86-132">JSON representation</span></span>

<span data-ttu-id="91c86-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91c86-133">Here is a JSON representation of the resource.</span></span>

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
