---
title: Тип ресурса Персонвебсите
description: Тип ресурса Персонвебсите
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4e37e769832340676f0d206b6727a57ce9809361
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227704"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="abac0-103">Тип ресурса Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="abac0-103">personWebsite resource type</span></span>

<span data-ttu-id="abac0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abac0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abac0-105">Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="abac0-105">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="abac0-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="abac0-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="abac0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="abac0-107">Methods</span></span>

| <span data-ttu-id="abac0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="abac0-108">Method</span></span>                                                         | <span data-ttu-id="abac0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="abac0-109">Return Type</span></span>                       | <span data-ttu-id="abac0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="abac0-110">Description</span></span>                                                          |
|:---------------------------------------------------------------|:----------------------------------|:---------------------------------------------------------------------|
| [<span data-ttu-id="abac0-111">Получение Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="abac0-111">Get personWebsite</span></span>](../api/personwebsite-get.md)               | [<span data-ttu-id="abac0-112">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="abac0-112">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="abac0-113">Чтение свойств и связей объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="abac0-113">Read the properties and relationships of a **personWebsite** object.</span></span> |
| [<span data-ttu-id="abac0-114">Обновление Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="abac0-114">Update personWebsite</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="abac0-115">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="abac0-115">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="abac0-116">Обновление объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="abac0-116">Update a **personWebsite** object.</span></span>                                   |
| [<span data-ttu-id="abac0-117">Удаление Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="abac0-117">Delete personWebsite</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="abac0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="abac0-118">None</span></span>                              | <span data-ttu-id="abac0-119">Удаление объекта **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="abac0-119">Delete a **personWebsite** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="abac0-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="abac0-120">Properties</span></span>

| <span data-ttu-id="abac0-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="abac0-121">Property</span></span>     | <span data-ttu-id="abac0-122">Тип</span><span class="sxs-lookup"><span data-stu-id="abac0-122">Type</span></span>              | <span data-ttu-id="abac0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="abac0-123">Description</span></span>                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|<span data-ttu-id="abac0-124">categories</span><span class="sxs-lookup"><span data-stu-id="abac0-124">categories</span></span>    |<span data-ttu-id="abac0-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="abac0-125">String collection</span></span>  | <span data-ttu-id="abac0-126">Содержит категории, связанные с веб-сайтом пользователя (например, персональный, рецепты).</span><span class="sxs-lookup"><span data-stu-id="abac0-126">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="abac0-127">description</span><span class="sxs-lookup"><span data-stu-id="abac0-127">description</span></span>   |<span data-ttu-id="abac0-128">String</span><span class="sxs-lookup"><span data-stu-id="abac0-128">String</span></span>             | <span data-ttu-id="abac0-129">Содержит описание веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="abac0-129">Contains a description of the website.</span></span>                                                        |
|<span data-ttu-id="abac0-130">displayName</span><span class="sxs-lookup"><span data-stu-id="abac0-130">displayName</span></span>   |<span data-ttu-id="abac0-131">Строка</span><span class="sxs-lookup"><span data-stu-id="abac0-131">String</span></span>             | <span data-ttu-id="abac0-132">Содержит понятное имя для веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="abac0-132">Contains a friendly name for the website.</span></span>                                                     |
|<span data-ttu-id="abac0-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="abac0-133">webUrl</span></span>        |<span data-ttu-id="abac0-134">String</span><span class="sxs-lookup"><span data-stu-id="abac0-134">String</span></span>             | <span data-ttu-id="abac0-135">Содержит ссылку на сам веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="abac0-135">Contains a link to the website itself.</span></span>                                                        |

## <a name="relationships"></a><span data-ttu-id="abac0-136">Связи</span><span class="sxs-lookup"><span data-stu-id="abac0-136">Relationships</span></span>

<span data-ttu-id="abac0-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="abac0-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="abac0-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="abac0-138">JSON representation</span></span>

<span data-ttu-id="abac0-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abac0-139">The following is a JSON representation of the resource.</span></span>

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
