---
title: Тип ресурса Воркпоситион
description: Тип ресурса Воркпоситион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2a0d742d289cefac825155a2e8917365c0bb97af
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950467"
---
# <a name="workposition-resource-type"></a><span data-ttu-id="57b18-103">Тип ресурса Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="57b18-103">workPosition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57b18-104">Представляет подробные сведения о должностных единицах, связанных с [профилем](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="57b18-104">Represents detailed information about work positions associated with a user's [profile](profile.md).</span></span>

<span data-ttu-id="57b18-105">Этот тип ресурса наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="57b18-105">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="57b18-106">Методы</span><span class="sxs-lookup"><span data-stu-id="57b18-106">Methods</span></span>

| <span data-ttu-id="57b18-107">Метод</span><span class="sxs-lookup"><span data-stu-id="57b18-107">Method</span></span>                                         | <span data-ttu-id="57b18-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="57b18-108">Return Type</span></span>                     | <span data-ttu-id="57b18-109">Описание</span><span class="sxs-lookup"><span data-stu-id="57b18-109">Description</span></span>                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [<span data-ttu-id="57b18-110">Получение Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="57b18-110">Get workPosition</span></span>](../api/workposition-get.md) | [<span data-ttu-id="57b18-111">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="57b18-111">workPosition</span></span>](workposition.md) | <span data-ttu-id="57b18-112">Чтение свойств и связей объекта **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="57b18-112">Read the properties and relationships of a **workPosition** object.</span></span> |
| [<span data-ttu-id="57b18-113">Обновление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="57b18-113">Update workPosition</span></span>](../api/workposition-update.md)        | [<span data-ttu-id="57b18-114">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="57b18-114">workPosition</span></span>](workposition.md) | <span data-ttu-id="57b18-115">Обновление объекта **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="57b18-115">Update a **workPosition** object.</span></span>                               |
| [<span data-ttu-id="57b18-116">Удаление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="57b18-116">Delete workPosition</span></span>](../api/workposition-delete.md)        | <span data-ttu-id="57b18-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="57b18-117">None</span></span>                            | <span data-ttu-id="57b18-118">Удаление объекта **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="57b18-118">Delete a **workPosition** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="57b18-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="57b18-119">Properties</span></span>

| <span data-ttu-id="57b18-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="57b18-120">Property</span></span>             | <span data-ttu-id="57b18-121">Тип</span><span class="sxs-lookup"><span data-stu-id="57b18-121">Type</span></span>                               | <span data-ttu-id="57b18-122">Описание</span><span class="sxs-lookup"><span data-stu-id="57b18-122">Description</span></span>                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="57b18-123">categories</span><span class="sxs-lookup"><span data-stu-id="57b18-123">categories</span></span>            |<span data-ttu-id="57b18-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57b18-124">String collection</span></span>                   | <span data-ttu-id="57b18-125">Содержит категории, связанные с положением пользователя (например, цифровое преобразование, люди).</span><span class="sxs-lookup"><span data-stu-id="57b18-125">Contains categories a user has associated with the position (for example, digital transformation, people).</span></span> |
|<span data-ttu-id="57b18-126">описаны</span><span class="sxs-lookup"><span data-stu-id="57b18-126">detail</span></span>                |[<span data-ttu-id="57b18-127">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="57b18-127">positionDetail</span></span>](positiondetail.md) | <span data-ttu-id="57b18-128">Содержит подробные сведения о текущей и предыдущей позиции найма пользователя.</span><span class="sxs-lookup"><span data-stu-id="57b18-128">Contains detail about the user's current and previous employment positions.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="57b18-129">Связи</span><span class="sxs-lookup"><span data-stu-id="57b18-129">Relationships</span></span>

<span data-ttu-id="57b18-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="57b18-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57b18-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="57b18-131">JSON representation</span></span>

<span data-ttu-id="57b18-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57b18-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workPosition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
