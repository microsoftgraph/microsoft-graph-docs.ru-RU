---
title: Тип ресурса Воркбукранжефилл
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 60f2af8ce43dcba1866949864e581b4c933ee760
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046226"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="47129-103">Тип ресурса Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="47129-103">workbookRangeFill resource type</span></span>

<span data-ttu-id="47129-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47129-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47129-105">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="47129-105">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="47129-106">Методы</span><span class="sxs-lookup"><span data-stu-id="47129-106">Methods</span></span>

| <span data-ttu-id="47129-107">Метод</span><span class="sxs-lookup"><span data-stu-id="47129-107">Method</span></span>           | <span data-ttu-id="47129-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="47129-108">Return Type</span></span>    |<span data-ttu-id="47129-109">Описание</span><span class="sxs-lookup"><span data-stu-id="47129-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47129-110">Получение Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="47129-110">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="47129-111">воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="47129-111">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="47129-112">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="47129-112">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="47129-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="47129-113">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="47129-114">воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="47129-114">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="47129-115">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="47129-115">Update RangeFill object.</span></span> |
|[<span data-ttu-id="47129-116">Clear</span><span class="sxs-lookup"><span data-stu-id="47129-116">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="47129-117">Нет</span><span class="sxs-lookup"><span data-stu-id="47129-117">None</span></span>|<span data-ttu-id="47129-118">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="47129-118">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="47129-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="47129-119">Properties</span></span>
| <span data-ttu-id="47129-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="47129-120">Property</span></span>     | <span data-ttu-id="47129-121">Тип</span><span class="sxs-lookup"><span data-stu-id="47129-121">Type</span></span>   |<span data-ttu-id="47129-122">Описание</span><span class="sxs-lookup"><span data-stu-id="47129-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47129-123">color</span><span class="sxs-lookup"><span data-stu-id="47129-123">color</span></span>|<span data-ttu-id="47129-124">string</span><span class="sxs-lookup"><span data-stu-id="47129-124">string</span></span>|<span data-ttu-id="47129-125">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="47129-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="47129-126">Связи</span><span class="sxs-lookup"><span data-stu-id="47129-126">Relationships</span></span>
<span data-ttu-id="47129-127">Нет</span><span class="sxs-lookup"><span data-stu-id="47129-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="47129-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47129-128">JSON representation</span></span>

<span data-ttu-id="47129-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47129-129">Here is a JSON representation of the resource.</span></span>

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


