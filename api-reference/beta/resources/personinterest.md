---
title: Тип ресурса Персонинтерест
description: Тип ресурса Персонинтерест
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 05918edf82712d5253403ed63312eb941be14103
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949510"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="642c5-103">Тип ресурса Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="642c5-103">personInterest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="642c5-104">Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.</span><span class="sxs-lookup"><span data-stu-id="642c5-104">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="642c5-105">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="642c5-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="642c5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="642c5-106">Methods</span></span>

| <span data-ttu-id="642c5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="642c5-107">Method</span></span>       | <span data-ttu-id="642c5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="642c5-108">Return Type</span></span> | <span data-ttu-id="642c5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="642c5-109">Description</span></span> |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [<span data-ttu-id="642c5-110">Получение Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="642c5-110">Get personInterest</span></span>](../api/personinterest-get.md) | [<span data-ttu-id="642c5-111">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="642c5-111">personInterest</span></span>](personinterest.md) | <span data-ttu-id="642c5-112">Чтение свойств и связей объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="642c5-112">Read the properties and relationships of a **personInterest** object.</span></span> |
| [<span data-ttu-id="642c5-113">Обновление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="642c5-113">Update personInterest</span></span>](../api/personinterest-update.md)          | [<span data-ttu-id="642c5-114">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="642c5-114">personInterest</span></span>](personinterest.md) | <span data-ttu-id="642c5-115">Обновление объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="642c5-115">Update a **personInterest** object.</span></span>                               |
| [<span data-ttu-id="642c5-116">Удаление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="642c5-116">Delete personInterest</span></span>](../api/personinterest-delete.md)          | <span data-ttu-id="642c5-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="642c5-117">None</span></span>                                | <span data-ttu-id="642c5-118">Удаление объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="642c5-118">Delete a **personInterest** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="642c5-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="642c5-119">Properties</span></span>

| <span data-ttu-id="642c5-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="642c5-120">Property</span></span>     | <span data-ttu-id="642c5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="642c5-121">Type</span></span>             | <span data-ttu-id="642c5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="642c5-122">Description</span></span>                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|<span data-ttu-id="642c5-123">categories</span><span class="sxs-lookup"><span data-stu-id="642c5-123">categories</span></span>    |<span data-ttu-id="642c5-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="642c5-124">String collection</span></span> | <span data-ttu-id="642c5-125">Содержит категории, которые пользователь связал с интересом (например, персональный, реЦипиес).</span><span class="sxs-lookup"><span data-stu-id="642c5-125">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="642c5-126">description</span><span class="sxs-lookup"><span data-stu-id="642c5-126">description</span></span>   |<span data-ttu-id="642c5-127">String</span><span class="sxs-lookup"><span data-stu-id="642c5-127">String</span></span>            | <span data-ttu-id="642c5-128">Содержит описание интереса.</span><span class="sxs-lookup"><span data-stu-id="642c5-128">Contains a description of the interest.</span></span>                                              |
|<span data-ttu-id="642c5-129">displayName</span><span class="sxs-lookup"><span data-stu-id="642c5-129">displayName</span></span>   |<span data-ttu-id="642c5-130">Строка</span><span class="sxs-lookup"><span data-stu-id="642c5-130">String</span></span>            | <span data-ttu-id="642c5-131">Содержит понятное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="642c5-131">Contains a friendly name for the interest.</span></span>                                           |
|<span data-ttu-id="642c5-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="642c5-132">webUrl</span></span>        |<span data-ttu-id="642c5-133">String</span><span class="sxs-lookup"><span data-stu-id="642c5-133">String</span></span>            | <span data-ttu-id="642c5-134">Содержит ссылку на веб-страницу или ресурс, представляющие интерес.</span><span class="sxs-lookup"><span data-stu-id="642c5-134">Contains a link to a web page or resource about the interest.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="642c5-135">Связи</span><span class="sxs-lookup"><span data-stu-id="642c5-135">Relationships</span></span>

<span data-ttu-id="642c5-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="642c5-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="642c5-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="642c5-137">JSON representation</span></span>

<span data-ttu-id="642c5-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="642c5-138">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
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
  "description": "personInterest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
