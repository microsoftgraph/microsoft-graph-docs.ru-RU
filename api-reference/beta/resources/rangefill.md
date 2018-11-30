---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
ms.openlocfilehash: 11806d95900c6e4ea1d4bf6ce4f4800bf5f6f66b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081646"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="72940-103">Тип ресурса RangeFill</span><span class="sxs-lookup"><span data-stu-id="72940-103">RangeFill resource type</span></span>

> <span data-ttu-id="72940-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72940-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72940-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72940-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72940-106">Представляет фон объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="72940-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="72940-107">Методы</span><span class="sxs-lookup"><span data-stu-id="72940-107">Methods</span></span>

| <span data-ttu-id="72940-108">Метод</span><span class="sxs-lookup"><span data-stu-id="72940-108">Method</span></span>           | <span data-ttu-id="72940-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72940-109">Return Type</span></span>    |<span data-ttu-id="72940-110">Описание</span><span class="sxs-lookup"><span data-stu-id="72940-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72940-111">Получение объекта RangeFill</span><span class="sxs-lookup"><span data-stu-id="72940-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="72940-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="72940-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="72940-113">Чтение свойств и связей объекта rangeFill.</span><span class="sxs-lookup"><span data-stu-id="72940-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="72940-114">Update</span><span class="sxs-lookup"><span data-stu-id="72940-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="72940-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="72940-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="72940-116">Обновление объекта RangeFill.</span><span class="sxs-lookup"><span data-stu-id="72940-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="72940-117">Clear</span><span class="sxs-lookup"><span data-stu-id="72940-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="72940-118">Нет</span><span class="sxs-lookup"><span data-stu-id="72940-118">None</span></span>|<span data-ttu-id="72940-119">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="72940-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="72940-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="72940-120">Properties</span></span>
| <span data-ttu-id="72940-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="72940-121">Property</span></span>     | <span data-ttu-id="72940-122">Тип</span><span class="sxs-lookup"><span data-stu-id="72940-122">Type</span></span>   |<span data-ttu-id="72940-123">Описание</span><span class="sxs-lookup"><span data-stu-id="72940-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72940-124">color</span><span class="sxs-lookup"><span data-stu-id="72940-124">color</span></span>|<span data-ttu-id="72940-125">строка</span><span class="sxs-lookup"><span data-stu-id="72940-125">string</span></span>|<span data-ttu-id="72940-126">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="72940-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="72940-127">Связи</span><span class="sxs-lookup"><span data-stu-id="72940-127">Relationships</span></span>
<span data-ttu-id="72940-128">Нет</span><span class="sxs-lookup"><span data-stu-id="72940-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="72940-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72940-129">JSON representation</span></span>

<span data-ttu-id="72940-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72940-130">Here is a JSON representation of the resource.</span></span>

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