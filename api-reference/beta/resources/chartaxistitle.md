---
title: Тип ресурса ChartAxisTitle
description: Представляет название оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a78219e5833f7f85cde571dc984959b642ebe4d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894182"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="11407-103">Тип ресурса ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="11407-103">ChartAxisTitle resource type</span></span>

> <span data-ttu-id="11407-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11407-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11407-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11407-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11407-106">Представляет название оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="11407-106">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="11407-107">Методы</span><span class="sxs-lookup"><span data-stu-id="11407-107">Methods</span></span>

| <span data-ttu-id="11407-108">Метод</span><span class="sxs-lookup"><span data-stu-id="11407-108">Method</span></span>           | <span data-ttu-id="11407-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11407-109">Return Type</span></span>    |<span data-ttu-id="11407-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11407-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11407-111">Получение объекта ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="11407-111">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="11407-112">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="11407-112">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="11407-113">Чтение свойств и связей объекта chartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="11407-113">Read properties and relationships of chartAxisTitle object.</span></span>|
|<span data-ttu-id="11407-114">[обновление](../api/chartaxistitle-update.md).</span><span class="sxs-lookup"><span data-stu-id="11407-114">[Update](../api/chartaxistitle-update.md)</span></span> | [<span data-ttu-id="11407-115">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="11407-115">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="11407-116">Обновление объекта ChartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="11407-116">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="11407-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="11407-117">Properties</span></span>
| <span data-ttu-id="11407-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="11407-118">Property</span></span>     | <span data-ttu-id="11407-119">Тип</span><span class="sxs-lookup"><span data-stu-id="11407-119">Type</span></span>   |<span data-ttu-id="11407-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11407-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11407-121">text</span><span class="sxs-lookup"><span data-stu-id="11407-121">text</span></span>|<span data-ttu-id="11407-122">строка</span><span class="sxs-lookup"><span data-stu-id="11407-122">string</span></span>|<span data-ttu-id="11407-123">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="11407-123">Represents the axis title.</span></span>|
|<span data-ttu-id="11407-124">visible</span><span class="sxs-lookup"><span data-stu-id="11407-124">visible</span></span>|<span data-ttu-id="11407-125">boolean</span><span class="sxs-lookup"><span data-stu-id="11407-125">boolean</span></span>|<span data-ttu-id="11407-126">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="11407-126">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11407-127">Связи</span><span class="sxs-lookup"><span data-stu-id="11407-127">Relationships</span></span>
| <span data-ttu-id="11407-128">Связь</span><span class="sxs-lookup"><span data-stu-id="11407-128">Relationship</span></span> | <span data-ttu-id="11407-129">Тип</span><span class="sxs-lookup"><span data-stu-id="11407-129">Type</span></span>   |<span data-ttu-id="11407-130">Описание</span><span class="sxs-lookup"><span data-stu-id="11407-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11407-131">format</span><span class="sxs-lookup"><span data-stu-id="11407-131">format</span></span>|[<span data-ttu-id="11407-132">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="11407-132">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="11407-p102">Представляет форматирование для названия оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11407-p102">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11407-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11407-135">JSON representation</span></span>

<span data-ttu-id="11407-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11407-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
