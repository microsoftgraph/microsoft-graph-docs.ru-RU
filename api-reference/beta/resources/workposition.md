---
title: Тип ресурса Воркпоситион
description: Тип ресурса Воркпоситион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 086273e54d923054ce8e71ef1c67fb2bb4f7002a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519066"
---
# <a name="workposition-resource-type"></a><span data-ttu-id="fb310-103">Тип ресурса Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="fb310-103">workPosition resource type</span></span>

<span data-ttu-id="fb310-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fb310-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb310-105">Представляет подробные сведения о должностных единицах, связанных с [профилем](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="fb310-105">Represents detailed information about work positions associated with a user's [profile](profile.md).</span></span>

<span data-ttu-id="fb310-106">Этот тип ресурса наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fb310-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fb310-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fb310-107">Methods</span></span>

| <span data-ttu-id="fb310-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fb310-108">Method</span></span>                                         | <span data-ttu-id="fb310-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb310-109">Return Type</span></span>                     | <span data-ttu-id="fb310-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb310-110">Description</span></span>                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [<span data-ttu-id="fb310-111">Получение Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="fb310-111">Get workPosition</span></span>](../api/workposition-get.md) | [<span data-ttu-id="fb310-112">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="fb310-112">workPosition</span></span>](workposition.md) | <span data-ttu-id="fb310-113">Чтение свойств и связей объекта **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="fb310-113">Read the properties and relationships of a **workPosition** object.</span></span> |
| [<span data-ttu-id="fb310-114">Обновление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="fb310-114">Update workPosition</span></span>](../api/workposition-update.md)        | [<span data-ttu-id="fb310-115">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="fb310-115">workPosition</span></span>](workposition.md) | <span data-ttu-id="fb310-116">Обновление объекта **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="fb310-116">Update a **workPosition** object.</span></span>                               |
| [<span data-ttu-id="fb310-117">Удаление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="fb310-117">Delete workPosition</span></span>](../api/workposition-delete.md)        | <span data-ttu-id="fb310-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fb310-118">None</span></span>                            | <span data-ttu-id="fb310-119">Удаление объекта **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="fb310-119">Delete a **workPosition** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="fb310-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb310-120">Properties</span></span>

| <span data-ttu-id="fb310-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb310-121">Property</span></span>             | <span data-ttu-id="fb310-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fb310-122">Type</span></span>                               | <span data-ttu-id="fb310-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fb310-123">Description</span></span>                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="fb310-124">categories</span><span class="sxs-lookup"><span data-stu-id="fb310-124">categories</span></span>            |<span data-ttu-id="fb310-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb310-125">String collection</span></span>                   | <span data-ttu-id="fb310-126">Содержит категории, связанные с положением пользователя (например, цифровое преобразование, люди).</span><span class="sxs-lookup"><span data-stu-id="fb310-126">Contains categories a user has associated with the position (for example, digital transformation, people).</span></span> |
|<span data-ttu-id="fb310-127">описаны</span><span class="sxs-lookup"><span data-stu-id="fb310-127">detail</span></span>                |[<span data-ttu-id="fb310-128">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="fb310-128">positionDetail</span></span>](positiondetail.md) | <span data-ttu-id="fb310-129">Содержит подробные сведения о текущей и предыдущей позиции найма пользователя.</span><span class="sxs-lookup"><span data-stu-id="fb310-129">Contains detail about the user's current and previous employment positions.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="fb310-130">Связи</span><span class="sxs-lookup"><span data-stu-id="fb310-130">Relationships</span></span>

<span data-ttu-id="fb310-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fb310-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb310-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fb310-132">JSON representation</span></span>

<span data-ttu-id="fb310-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb310-133">The following is a JSON representation of the resource.</span></span>

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
