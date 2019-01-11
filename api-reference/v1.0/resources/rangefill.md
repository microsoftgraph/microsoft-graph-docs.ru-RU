---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d1dc1bda19d725999f9a49644bee1e4cb1126ec2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877191"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="7c95d-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="7c95d-103">RangeFill resource type</span></span>

<span data-ttu-id="7c95d-104">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="7c95d-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="7c95d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7c95d-105">Methods</span></span>

| <span data-ttu-id="7c95d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7c95d-106">Method</span></span>           | <span data-ttu-id="7c95d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c95d-107">Return Type</span></span>    |<span data-ttu-id="7c95d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c95d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c95d-109">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="7c95d-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="7c95d-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="7c95d-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="7c95d-111">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="7c95d-111">Read properties and relationships of rangeFill object.</span></span>|
|<span data-ttu-id="7c95d-112">[обновление](../api/rangefill-update.md).</span><span class="sxs-lookup"><span data-stu-id="7c95d-112">[Update](../api/rangefill-update.md)</span></span> | [<span data-ttu-id="7c95d-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="7c95d-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="7c95d-114">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="7c95d-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="7c95d-115">Clear</span><span class="sxs-lookup"><span data-stu-id="7c95d-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="7c95d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="7c95d-116">None</span></span>|<span data-ttu-id="7c95d-117">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="7c95d-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c95d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c95d-118">Properties</span></span>
| <span data-ttu-id="7c95d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c95d-119">Property</span></span>     | <span data-ttu-id="7c95d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7c95d-120">Type</span></span>   |<span data-ttu-id="7c95d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7c95d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c95d-122">color</span><span class="sxs-lookup"><span data-stu-id="7c95d-122">color</span></span>|<span data-ttu-id="7c95d-123">строка</span><span class="sxs-lookup"><span data-stu-id="7c95d-123">string</span></span>|<span data-ttu-id="7c95d-124">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="7c95d-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c95d-125">Связи</span><span class="sxs-lookup"><span data-stu-id="7c95d-125">Relationships</span></span>
<span data-ttu-id="7c95d-126">Нет</span><span class="sxs-lookup"><span data-stu-id="7c95d-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7c95d-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c95d-127">JSON representation</span></span>

<span data-ttu-id="7c95d-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c95d-128">Here is a JSON representation of the resource.</span></span>

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
