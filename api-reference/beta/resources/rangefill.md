---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1ae60c0b362ba8593f374c5edd505121cd18587
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509674"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="40366-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="40366-103">RangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40366-104">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="40366-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="40366-105">Методы</span><span class="sxs-lookup"><span data-stu-id="40366-105">Methods</span></span>

| <span data-ttu-id="40366-106">Метод</span><span class="sxs-lookup"><span data-stu-id="40366-106">Method</span></span>           | <span data-ttu-id="40366-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="40366-107">Return Type</span></span>    |<span data-ttu-id="40366-108">Описание</span><span class="sxs-lookup"><span data-stu-id="40366-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40366-109">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="40366-109">[Get RangeFill](../api/rangefill-get.md)</span></span> | <span data-ttu-id="40366-110">RangeFill</span><span class="sxs-lookup"><span data-stu-id="40366-110">[RangeFill](rangefill.md)</span></span> |<span data-ttu-id="40366-111">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="40366-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="40366-112">Update</span><span class="sxs-lookup"><span data-stu-id="40366-112">Update</span></span>](../api/rangefill-update.md) | <span data-ttu-id="40366-113">RangeFill</span><span class="sxs-lookup"><span data-stu-id="40366-113">[RangeFill](rangefill.md)</span></span>   |<span data-ttu-id="40366-114">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="40366-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="40366-115">Clear</span><span class="sxs-lookup"><span data-stu-id="40366-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="40366-116">Нет</span><span class="sxs-lookup"><span data-stu-id="40366-116">None</span></span>|<span data-ttu-id="40366-117">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="40366-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="40366-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="40366-118">Properties</span></span>
| <span data-ttu-id="40366-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="40366-119">Property</span></span>     | <span data-ttu-id="40366-120">Тип</span><span class="sxs-lookup"><span data-stu-id="40366-120">Type</span></span>   |<span data-ttu-id="40366-121">Описание</span><span class="sxs-lookup"><span data-stu-id="40366-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40366-122">color</span><span class="sxs-lookup"><span data-stu-id="40366-122">color</span></span>|<span data-ttu-id="40366-123">строка</span><span class="sxs-lookup"><span data-stu-id="40366-123">string</span></span>|<span data-ttu-id="40366-124">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="40366-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="40366-125">Связи</span><span class="sxs-lookup"><span data-stu-id="40366-125">Relationships</span></span>
<span data-ttu-id="40366-126">Нет</span><span class="sxs-lookup"><span data-stu-id="40366-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="40366-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40366-127">JSON representation</span></span>

<span data-ttu-id="40366-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40366-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefill.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
