---
title: Тип ресурса Персонвебсите
description: Тип ресурса Персонвебсите
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b5e6b8c3013c647087ab3d8db28b0196d0c79036
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949505"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="24c49-103">Тип ресурса Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="24c49-103">personWebsite resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24c49-104">Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="24c49-104">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="24c49-105">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="24c49-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="24c49-106">Методы</span><span class="sxs-lookup"><span data-stu-id="24c49-106">Methods</span></span>

| <span data-ttu-id="24c49-107">Метод</span><span class="sxs-lookup"><span data-stu-id="24c49-107">Method</span></span>                                           | <span data-ttu-id="24c49-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24c49-108">Return Type</span></span>                       | <span data-ttu-id="24c49-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24c49-109">Description</span></span>                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [<span data-ttu-id="24c49-110">Получение Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="24c49-110">Get personWebsite</span></span>](../api/personwebsite-get.md) | [<span data-ttu-id="24c49-111">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="24c49-111">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="24c49-112">Чтение свойств и связей объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="24c49-112">Read the properties and relationships of a **personWebsite** object.</span></span> |
| [<span data-ttu-id="24c49-113">Обновление Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="24c49-113">Update personWebsite</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="24c49-114">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="24c49-114">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="24c49-115">Обновление объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="24c49-115">Update a **personWebsite** object.</span></span>                               |
| [<span data-ttu-id="24c49-116">Удаление Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="24c49-116">Delete personWebsite</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="24c49-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="24c49-117">None</span></span>                              | <span data-ttu-id="24c49-118">Удаление объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="24c49-118">Delete a **personWebsite** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="24c49-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="24c49-119">Properties</span></span>

| <span data-ttu-id="24c49-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="24c49-120">Property</span></span>     | <span data-ttu-id="24c49-121">Тип</span><span class="sxs-lookup"><span data-stu-id="24c49-121">Type</span></span>              | <span data-ttu-id="24c49-122">Описание</span><span class="sxs-lookup"><span data-stu-id="24c49-122">Description</span></span>                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="24c49-123">categories</span><span class="sxs-lookup"><span data-stu-id="24c49-123">categories</span></span>    |<span data-ttu-id="24c49-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="24c49-124">String collection</span></span>  | <span data-ttu-id="24c49-125">Содержит категории, связанные с веб-сайтом пользователя (например, персональный, рецепты).</span><span class="sxs-lookup"><span data-stu-id="24c49-125">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="24c49-126">description</span><span class="sxs-lookup"><span data-stu-id="24c49-126">description</span></span>   |<span data-ttu-id="24c49-127">String</span><span class="sxs-lookup"><span data-stu-id="24c49-127">String</span></span>             | <span data-ttu-id="24c49-128">Содержит описание веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="24c49-128">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="24c49-129">displayName</span><span class="sxs-lookup"><span data-stu-id="24c49-129">displayName</span></span>   |<span data-ttu-id="24c49-130">Строка</span><span class="sxs-lookup"><span data-stu-id="24c49-130">String</span></span>             | <span data-ttu-id="24c49-131">Содержит понятное имя для веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="24c49-131">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="24c49-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="24c49-132">webUrl</span></span>        |<span data-ttu-id="24c49-133">String</span><span class="sxs-lookup"><span data-stu-id="24c49-133">String</span></span>             | <span data-ttu-id="24c49-134">Содержит ссылку на сам веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="24c49-134">Contains a link to the website itself.</span></span>                                              |

## <a name="relationships"></a><span data-ttu-id="24c49-135">Связи</span><span class="sxs-lookup"><span data-stu-id="24c49-135">Relationships</span></span>

<span data-ttu-id="24c49-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24c49-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24c49-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24c49-137">JSON representation</span></span>

<span data-ttu-id="24c49-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24c49-138">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personWebsite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
