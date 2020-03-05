---
title: Тип ресурса Персонвебсите
description: Тип ресурса Персонвебсите
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cf4386cf70179715880a1ae07db3dfbb5f07c224
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521899"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="3df07-103">Тип ресурса Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="3df07-103">personWebsite resource type</span></span>

<span data-ttu-id="3df07-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3df07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3df07-105">Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="3df07-105">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="3df07-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3df07-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3df07-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3df07-107">Methods</span></span>

| <span data-ttu-id="3df07-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3df07-108">Method</span></span>                                           | <span data-ttu-id="3df07-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3df07-109">Return Type</span></span>                       | <span data-ttu-id="3df07-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3df07-110">Description</span></span>                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [<span data-ttu-id="3df07-111">Получение Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="3df07-111">Get personWebsite</span></span>](../api/personwebsite-get.md) | [<span data-ttu-id="3df07-112">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="3df07-112">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="3df07-113">Чтение свойств и связей объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="3df07-113">Read the properties and relationships of a **personWebsite** object.</span></span> |
| [<span data-ttu-id="3df07-114">Обновление Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="3df07-114">Update personWebsite</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="3df07-115">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="3df07-115">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="3df07-116">Обновление объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="3df07-116">Update a **personWebsite** object.</span></span>                               |
| [<span data-ttu-id="3df07-117">Удаление Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="3df07-117">Delete personWebsite</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="3df07-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3df07-118">None</span></span>                              | <span data-ttu-id="3df07-119">Удаление объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="3df07-119">Delete a **personWebsite** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="3df07-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="3df07-120">Properties</span></span>

| <span data-ttu-id="3df07-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="3df07-121">Property</span></span>     | <span data-ttu-id="3df07-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3df07-122">Type</span></span>              | <span data-ttu-id="3df07-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3df07-123">Description</span></span>                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="3df07-124">categories</span><span class="sxs-lookup"><span data-stu-id="3df07-124">categories</span></span>    |<span data-ttu-id="3df07-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3df07-125">String collection</span></span>  | <span data-ttu-id="3df07-126">Содержит категории, связанные с веб-сайтом пользователя (например, персональный, рецепты).</span><span class="sxs-lookup"><span data-stu-id="3df07-126">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="3df07-127">description</span><span class="sxs-lookup"><span data-stu-id="3df07-127">description</span></span>   |<span data-ttu-id="3df07-128">String</span><span class="sxs-lookup"><span data-stu-id="3df07-128">String</span></span>             | <span data-ttu-id="3df07-129">Содержит описание веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="3df07-129">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="3df07-130">displayName</span><span class="sxs-lookup"><span data-stu-id="3df07-130">displayName</span></span>   |<span data-ttu-id="3df07-131">Строка</span><span class="sxs-lookup"><span data-stu-id="3df07-131">String</span></span>             | <span data-ttu-id="3df07-132">Содержит понятное имя для веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="3df07-132">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="3df07-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="3df07-133">webUrl</span></span>        |<span data-ttu-id="3df07-134">String</span><span class="sxs-lookup"><span data-stu-id="3df07-134">String</span></span>             | <span data-ttu-id="3df07-135">Содержит ссылку на сам веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="3df07-135">Contains a link to the website itself.</span></span>                                              |

## <a name="relationships"></a><span data-ttu-id="3df07-136">Связи</span><span class="sxs-lookup"><span data-stu-id="3df07-136">Relationships</span></span>

<span data-ttu-id="3df07-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3df07-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3df07-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3df07-138">JSON representation</span></span>

<span data-ttu-id="3df07-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3df07-139">The following is a JSON representation of the resource.</span></span> 

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
