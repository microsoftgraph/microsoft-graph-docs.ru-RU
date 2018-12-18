---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
ms.openlocfilehash: 6ddd039190af0e86067dfda651b2bc387b4cf74f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303565"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="6c6e2-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="6c6e2-103">RangeFill resource type</span></span>

<span data-ttu-id="6c6e2-104">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="6c6e2-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="6c6e2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6c6e2-105">Methods</span></span>

| <span data-ttu-id="6c6e2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6c6e2-106">Method</span></span>           | <span data-ttu-id="6c6e2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c6e2-107">Return Type</span></span>    |<span data-ttu-id="6c6e2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6c6e2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c6e2-109">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="6c6e2-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="6c6e2-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="6c6e2-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="6c6e2-111">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="6c6e2-111">Read properties and relationships of rangeFill object.</span></span>|
|<span data-ttu-id="6c6e2-112">[обновление](../api/rangefill-update.md).</span><span class="sxs-lookup"><span data-stu-id="6c6e2-112">[Update](../api/rangefill-update.md)</span></span> | [<span data-ttu-id="6c6e2-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="6c6e2-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="6c6e2-114">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="6c6e2-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="6c6e2-115">Clear</span><span class="sxs-lookup"><span data-stu-id="6c6e2-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="6c6e2-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6c6e2-116">None</span></span>|<span data-ttu-id="6c6e2-117">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="6c6e2-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c6e2-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c6e2-118">Properties</span></span>
| <span data-ttu-id="6c6e2-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c6e2-119">Property</span></span>     | <span data-ttu-id="6c6e2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6c6e2-120">Type</span></span>   |<span data-ttu-id="6c6e2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6c6e2-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c6e2-122">color</span><span class="sxs-lookup"><span data-stu-id="6c6e2-122">color</span></span>|<span data-ttu-id="6c6e2-123">строка</span><span class="sxs-lookup"><span data-stu-id="6c6e2-123">string</span></span>|<span data-ttu-id="6c6e2-124">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="6c6e2-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c6e2-125">Связи</span><span class="sxs-lookup"><span data-stu-id="6c6e2-125">Relationships</span></span>
<span data-ttu-id="6c6e2-126">Нет</span><span class="sxs-lookup"><span data-stu-id="6c6e2-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6c6e2-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c6e2-127">JSON representation</span></span>

<span data-ttu-id="6c6e2-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c6e2-128">Here is a JSON representation of the resource.</span></span>

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