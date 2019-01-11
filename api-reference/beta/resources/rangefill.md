---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8ceab66373331b6e144b69119d521a3e5ddccdc7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817761"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="fd593-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="fd593-103">RangeFill resource type</span></span>

> <span data-ttu-id="fd593-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd593-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd593-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd593-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd593-106">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="fd593-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="fd593-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fd593-107">Methods</span></span>

| <span data-ttu-id="fd593-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fd593-108">Method</span></span>           | <span data-ttu-id="fd593-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fd593-109">Return Type</span></span>    |<span data-ttu-id="fd593-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fd593-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd593-111">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="fd593-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="fd593-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="fd593-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="fd593-113">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="fd593-113">Read properties and relationships of rangeFill object.</span></span>|
|<span data-ttu-id="fd593-114">[обновление](../api/rangefill-update.md).</span><span class="sxs-lookup"><span data-stu-id="fd593-114">[Update](../api/rangefill-update.md)</span></span> | [<span data-ttu-id="fd593-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="fd593-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="fd593-116">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="fd593-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="fd593-117">Clear</span><span class="sxs-lookup"><span data-stu-id="fd593-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="fd593-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fd593-118">None</span></span>|<span data-ttu-id="fd593-119">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="fd593-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd593-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd593-120">Properties</span></span>
| <span data-ttu-id="fd593-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd593-121">Property</span></span>     | <span data-ttu-id="fd593-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fd593-122">Type</span></span>   |<span data-ttu-id="fd593-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fd593-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd593-124">color</span><span class="sxs-lookup"><span data-stu-id="fd593-124">color</span></span>|<span data-ttu-id="fd593-125">строка</span><span class="sxs-lookup"><span data-stu-id="fd593-125">string</span></span>|<span data-ttu-id="fd593-126">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="fd593-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd593-127">Связи</span><span class="sxs-lookup"><span data-stu-id="fd593-127">Relationships</span></span>
<span data-ttu-id="fd593-128">Нет</span><span class="sxs-lookup"><span data-stu-id="fd593-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fd593-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd593-129">JSON representation</span></span>

<span data-ttu-id="fd593-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd593-130">Here is a JSON representation of the resource.</span></span>

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
