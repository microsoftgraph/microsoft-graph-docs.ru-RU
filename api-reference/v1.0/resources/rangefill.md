---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 75aa4bd91ad6f1038fdc42460c6a3c9ab928a09d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579475"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="670c0-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="670c0-103">RangeFill resource type</span></span>

<span data-ttu-id="670c0-104">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="670c0-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="670c0-105">Методы</span><span class="sxs-lookup"><span data-stu-id="670c0-105">Methods</span></span>

| <span data-ttu-id="670c0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="670c0-106">Method</span></span>           | <span data-ttu-id="670c0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="670c0-107">Return Type</span></span>    |<span data-ttu-id="670c0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="670c0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="670c0-109">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="670c0-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="670c0-110">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="670c0-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="670c0-111">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="670c0-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="670c0-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="670c0-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="670c0-113">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="670c0-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="670c0-114">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="670c0-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="670c0-115">Clear</span><span class="sxs-lookup"><span data-stu-id="670c0-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="670c0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="670c0-116">None</span></span>|<span data-ttu-id="670c0-117">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="670c0-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="670c0-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="670c0-118">Properties</span></span>
| <span data-ttu-id="670c0-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="670c0-119">Property</span></span>     | <span data-ttu-id="670c0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="670c0-120">Type</span></span>   |<span data-ttu-id="670c0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="670c0-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="670c0-122">color</span><span class="sxs-lookup"><span data-stu-id="670c0-122">color</span></span>|<span data-ttu-id="670c0-123">string</span><span class="sxs-lookup"><span data-stu-id="670c0-123">string</span></span>|<span data-ttu-id="670c0-124">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="670c0-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="670c0-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="670c0-125">Relationships</span></span>
<span data-ttu-id="670c0-126">Нет</span><span class="sxs-lookup"><span data-stu-id="670c0-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="670c0-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="670c0-127">JSON representation</span></span>

<span data-ttu-id="670c0-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="670c0-128">Here is a JSON representation of the resource.</span></span>

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
