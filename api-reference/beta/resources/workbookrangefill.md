---
title: Тип ресурса Воркбукранжефилл
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: cb61352964323b0ded8733aa52ddd19854e028d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007097"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="22275-103">Тип ресурса Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="22275-103">workbookRangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22275-104">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="22275-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="22275-105">Методы</span><span class="sxs-lookup"><span data-stu-id="22275-105">Methods</span></span>

| <span data-ttu-id="22275-106">Метод</span><span class="sxs-lookup"><span data-stu-id="22275-106">Method</span></span>           | <span data-ttu-id="22275-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22275-107">Return Type</span></span>    |<span data-ttu-id="22275-108">Описание</span><span class="sxs-lookup"><span data-stu-id="22275-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22275-109">Получение Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="22275-109">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="22275-110">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="22275-110">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="22275-111">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="22275-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="22275-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="22275-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="22275-113">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="22275-113">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="22275-114">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="22275-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="22275-115">Clear</span><span class="sxs-lookup"><span data-stu-id="22275-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="22275-116">Нет</span><span class="sxs-lookup"><span data-stu-id="22275-116">None</span></span>|<span data-ttu-id="22275-117">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="22275-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="22275-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="22275-118">Properties</span></span>
| <span data-ttu-id="22275-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="22275-119">Property</span></span>     | <span data-ttu-id="22275-120">Тип</span><span class="sxs-lookup"><span data-stu-id="22275-120">Type</span></span>   |<span data-ttu-id="22275-121">Описание</span><span class="sxs-lookup"><span data-stu-id="22275-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22275-122">color</span><span class="sxs-lookup"><span data-stu-id="22275-122">color</span></span>|<span data-ttu-id="22275-123">string</span><span class="sxs-lookup"><span data-stu-id="22275-123">string</span></span>|<span data-ttu-id="22275-124">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="22275-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="22275-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="22275-125">Relationships</span></span>
<span data-ttu-id="22275-126">Нет</span><span class="sxs-lookup"><span data-stu-id="22275-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="22275-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22275-127">JSON representation</span></span>

<span data-ttu-id="22275-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22275-128">Here is a JSON representation of the resource.</span></span>

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
