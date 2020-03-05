---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 37bc96fdd0dad65a1f6b5b6bcec244ef96b915ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447026"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="1951b-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="1951b-103">RangeFill resource type</span></span>

<span data-ttu-id="1951b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1951b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1951b-105">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="1951b-105">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="1951b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1951b-106">Methods</span></span>

| <span data-ttu-id="1951b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1951b-107">Method</span></span>           | <span data-ttu-id="1951b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1951b-108">Return Type</span></span>    |<span data-ttu-id="1951b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1951b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1951b-110">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="1951b-110">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="1951b-111">воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="1951b-111">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="1951b-112">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="1951b-112">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="1951b-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="1951b-113">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="1951b-114">воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="1951b-114">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="1951b-115">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="1951b-115">Update RangeFill object.</span></span> |
|[<span data-ttu-id="1951b-116">Clear</span><span class="sxs-lookup"><span data-stu-id="1951b-116">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="1951b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1951b-117">None</span></span>|<span data-ttu-id="1951b-118">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="1951b-118">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="1951b-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1951b-119">Properties</span></span>
| <span data-ttu-id="1951b-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1951b-120">Property</span></span>     | <span data-ttu-id="1951b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1951b-121">Type</span></span>   |<span data-ttu-id="1951b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1951b-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1951b-123">color</span><span class="sxs-lookup"><span data-stu-id="1951b-123">color</span></span>|<span data-ttu-id="1951b-124">string</span><span class="sxs-lookup"><span data-stu-id="1951b-124">string</span></span>|<span data-ttu-id="1951b-125">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="1951b-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="1951b-126">Связи</span><span class="sxs-lookup"><span data-stu-id="1951b-126">Relationships</span></span>
<span data-ttu-id="1951b-127">Нет</span><span class="sxs-lookup"><span data-stu-id="1951b-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1951b-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1951b-128">JSON representation</span></span>

<span data-ttu-id="1951b-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1951b-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
