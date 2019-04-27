---
title: Тип ресурса Воркбукранжефилл
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eea7337fa4aefb1bde607740b9a2fc78264dae91
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348977"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="2f737-103">Тип ресурса Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="2f737-103">workbookRangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f737-104">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="2f737-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="2f737-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2f737-105">Methods</span></span>

| <span data-ttu-id="2f737-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2f737-106">Method</span></span>           | <span data-ttu-id="2f737-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f737-107">Return Type</span></span>    |<span data-ttu-id="2f737-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2f737-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f737-109">Получение Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="2f737-109">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="2f737-110">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="2f737-110">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="2f737-111">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="2f737-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="2f737-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="2f737-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="2f737-113">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="2f737-113">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="2f737-114">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="2f737-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="2f737-115">Clear</span><span class="sxs-lookup"><span data-stu-id="2f737-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="2f737-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2f737-116">None</span></span>|<span data-ttu-id="2f737-117">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="2f737-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f737-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f737-118">Properties</span></span>
| <span data-ttu-id="2f737-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f737-119">Property</span></span>     | <span data-ttu-id="2f737-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2f737-120">Type</span></span>   |<span data-ttu-id="2f737-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2f737-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f737-122">color</span><span class="sxs-lookup"><span data-stu-id="2f737-122">color</span></span>|<span data-ttu-id="2f737-123">string</span><span class="sxs-lookup"><span data-stu-id="2f737-123">string</span></span>|<span data-ttu-id="2f737-124">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="2f737-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f737-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="2f737-125">Relationships</span></span>
<span data-ttu-id="2f737-126">Нет</span><span class="sxs-lookup"><span data-stu-id="2f737-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2f737-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f737-127">JSON representation</span></span>

<span data-ttu-id="2f737-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f737-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
