---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4043122f4c35c3e7f1c6f9d3919687833d35b9b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974345"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="73946-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="73946-103">RangeFill resource type</span></span>

> <span data-ttu-id="73946-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73946-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73946-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73946-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73946-106">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="73946-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="73946-107">Методы</span><span class="sxs-lookup"><span data-stu-id="73946-107">Methods</span></span>

| <span data-ttu-id="73946-108">Метод</span><span class="sxs-lookup"><span data-stu-id="73946-108">Method</span></span>           | <span data-ttu-id="73946-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="73946-109">Return Type</span></span>    |<span data-ttu-id="73946-110">Описание</span><span class="sxs-lookup"><span data-stu-id="73946-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73946-111">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="73946-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="73946-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="73946-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="73946-113">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="73946-113">Read properties and relationships of rangeFill object.</span></span>|
|<span data-ttu-id="73946-114">[обновление](../api/rangefill-update.md).</span><span class="sxs-lookup"><span data-stu-id="73946-114">[Update](../api/rangefill-update.md)</span></span> | [<span data-ttu-id="73946-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="73946-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="73946-116">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="73946-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="73946-117">Clear</span><span class="sxs-lookup"><span data-stu-id="73946-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="73946-118">Нет</span><span class="sxs-lookup"><span data-stu-id="73946-118">None</span></span>|<span data-ttu-id="73946-119">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="73946-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="73946-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="73946-120">Properties</span></span>
| <span data-ttu-id="73946-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="73946-121">Property</span></span>     | <span data-ttu-id="73946-122">Тип</span><span class="sxs-lookup"><span data-stu-id="73946-122">Type</span></span>   |<span data-ttu-id="73946-123">Описание</span><span class="sxs-lookup"><span data-stu-id="73946-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73946-124">color</span><span class="sxs-lookup"><span data-stu-id="73946-124">color</span></span>|<span data-ttu-id="73946-125">строка</span><span class="sxs-lookup"><span data-stu-id="73946-125">string</span></span>|<span data-ttu-id="73946-126">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="73946-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="73946-127">Связи</span><span class="sxs-lookup"><span data-stu-id="73946-127">Relationships</span></span>
<span data-ttu-id="73946-128">Нет</span><span class="sxs-lookup"><span data-stu-id="73946-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="73946-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73946-129">JSON representation</span></span>

<span data-ttu-id="73946-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73946-130">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
