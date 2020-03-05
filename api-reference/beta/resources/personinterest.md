---
title: Тип ресурса Персонинтерест
description: Тип ресурса Персонинтерест
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1da3ad429011da62f49105c6f352c86ec0741cd4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521913"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="d8c97-103">Тип ресурса Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="d8c97-103">personInterest resource type</span></span>

<span data-ttu-id="d8c97-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d8c97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8c97-105">Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.</span><span class="sxs-lookup"><span data-stu-id="d8c97-105">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="d8c97-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d8c97-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d8c97-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d8c97-107">Methods</span></span>

| <span data-ttu-id="d8c97-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d8c97-108">Method</span></span>       | <span data-ttu-id="d8c97-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8c97-109">Return Type</span></span> | <span data-ttu-id="d8c97-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8c97-110">Description</span></span> |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [<span data-ttu-id="d8c97-111">Получение Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="d8c97-111">Get personInterest</span></span>](../api/personinterest-get.md) | [<span data-ttu-id="d8c97-112">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="d8c97-112">personInterest</span></span>](personinterest.md) | <span data-ttu-id="d8c97-113">Чтение свойств и связей объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="d8c97-113">Read the properties and relationships of a **personInterest** object.</span></span> |
| [<span data-ttu-id="d8c97-114">Обновление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="d8c97-114">Update personInterest</span></span>](../api/personinterest-update.md)          | [<span data-ttu-id="d8c97-115">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="d8c97-115">personInterest</span></span>](personinterest.md) | <span data-ttu-id="d8c97-116">Обновление объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="d8c97-116">Update a **personInterest** object.</span></span>                               |
| [<span data-ttu-id="d8c97-117">Удаление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="d8c97-117">Delete personInterest</span></span>](../api/personinterest-delete.md)          | <span data-ttu-id="d8c97-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d8c97-118">None</span></span>                                | <span data-ttu-id="d8c97-119">Удаление объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="d8c97-119">Delete a **personInterest** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="d8c97-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8c97-120">Properties</span></span>

| <span data-ttu-id="d8c97-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8c97-121">Property</span></span>     | <span data-ttu-id="d8c97-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d8c97-122">Type</span></span>             | <span data-ttu-id="d8c97-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d8c97-123">Description</span></span>                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|<span data-ttu-id="d8c97-124">categories</span><span class="sxs-lookup"><span data-stu-id="d8c97-124">categories</span></span>    |<span data-ttu-id="d8c97-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d8c97-125">String collection</span></span> | <span data-ttu-id="d8c97-126">Содержит категории, которые пользователь связал с интересом (например, персональный, реЦипиес).</span><span class="sxs-lookup"><span data-stu-id="d8c97-126">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="d8c97-127">description</span><span class="sxs-lookup"><span data-stu-id="d8c97-127">description</span></span>   |<span data-ttu-id="d8c97-128">String</span><span class="sxs-lookup"><span data-stu-id="d8c97-128">String</span></span>            | <span data-ttu-id="d8c97-129">Содержит описание интереса.</span><span class="sxs-lookup"><span data-stu-id="d8c97-129">Contains a description of the interest.</span></span>                                              |
|<span data-ttu-id="d8c97-130">displayName</span><span class="sxs-lookup"><span data-stu-id="d8c97-130">displayName</span></span>   |<span data-ttu-id="d8c97-131">Строка</span><span class="sxs-lookup"><span data-stu-id="d8c97-131">String</span></span>            | <span data-ttu-id="d8c97-132">Содержит понятное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="d8c97-132">Contains a friendly name for the interest.</span></span>                                           |
|<span data-ttu-id="d8c97-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="d8c97-133">webUrl</span></span>        |<span data-ttu-id="d8c97-134">String</span><span class="sxs-lookup"><span data-stu-id="d8c97-134">String</span></span>            | <span data-ttu-id="d8c97-135">Содержит ссылку на веб-страницу или ресурс, представляющие интерес.</span><span class="sxs-lookup"><span data-stu-id="d8c97-135">Contains a link to a web page or resource about the interest.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="d8c97-136">Связи</span><span class="sxs-lookup"><span data-stu-id="d8c97-136">Relationships</span></span>

<span data-ttu-id="d8c97-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d8c97-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8c97-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d8c97-138">JSON representation</span></span>

<span data-ttu-id="d8c97-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8c97-139">The following is a JSON representation of the resource.</span></span> 

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
