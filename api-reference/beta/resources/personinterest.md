---
title: Тип ресурса Персонинтерест
description: Тип ресурса Персонинтерест
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ef2675b8c604115fc5e04a7747dc4c110d567604
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939027"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="3c94e-103">Тип ресурса Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="3c94e-103">personInterest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c94e-104">Тип ресурса [персонинтерест](personinterest.md) предоставляет подробные сведения о интересах, которые пользователь связал с самим собой в различных службах.</span><span class="sxs-lookup"><span data-stu-id="3c94e-104">The [personInterest](personinterest.md) resource type provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="3c94e-105">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3c94e-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3c94e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3c94e-106">Methods</span></span>

| <span data-ttu-id="3c94e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3c94e-107">Method</span></span>       | <span data-ttu-id="3c94e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3c94e-108">Return Type</span></span> | <span data-ttu-id="3c94e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3c94e-109">Description</span></span> |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [<span data-ttu-id="3c94e-110">Получение Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="3c94e-110">Get personInterest</span></span>](../api/personinterest-get.md) | [<span data-ttu-id="3c94e-111">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="3c94e-111">personInterest</span></span>](personinterest.md) | <span data-ttu-id="3c94e-112">Чтение свойств и связей объекта Персонинтерест.</span><span class="sxs-lookup"><span data-stu-id="3c94e-112">Read properties and relationships of personInterest object.</span></span> |
| [<span data-ttu-id="3c94e-113">Update</span><span class="sxs-lookup"><span data-stu-id="3c94e-113">Update</span></span>](../api/personinterest-update.md)          | [<span data-ttu-id="3c94e-114">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="3c94e-114">personInterest</span></span>](personinterest.md) | <span data-ttu-id="3c94e-115">Обновление объекта Персонинтерест.</span><span class="sxs-lookup"><span data-stu-id="3c94e-115">Update personInterest object.</span></span>                               |
| [<span data-ttu-id="3c94e-116">Delete</span><span class="sxs-lookup"><span data-stu-id="3c94e-116">Delete</span></span>](../api/personinterest-delete.md)          | <span data-ttu-id="3c94e-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="3c94e-117">None</span></span>                                | <span data-ttu-id="3c94e-118">Удаление объекта Персонинтерест.</span><span class="sxs-lookup"><span data-stu-id="3c94e-118">Delete personInterest object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="3c94e-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c94e-119">Properties</span></span>

| <span data-ttu-id="3c94e-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c94e-120">Property</span></span>     | <span data-ttu-id="3c94e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3c94e-121">Type</span></span>             | <span data-ttu-id="3c94e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3c94e-122">Description</span></span>                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|<span data-ttu-id="3c94e-123">categories</span><span class="sxs-lookup"><span data-stu-id="3c94e-123">categories</span></span>    |<span data-ttu-id="3c94e-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c94e-124">String collection</span></span> | <span data-ttu-id="3c94e-125">Содержит категории, которые пользователь связал с интересом (например: личное, реЦипиес)</span><span class="sxs-lookup"><span data-stu-id="3c94e-125">Contains categories a user has associated with the interest (eg: personal, recipies)</span></span> |
|<span data-ttu-id="3c94e-126">description</span><span class="sxs-lookup"><span data-stu-id="3c94e-126">description</span></span>   |<span data-ttu-id="3c94e-127">String</span><span class="sxs-lookup"><span data-stu-id="3c94e-127">String</span></span>            | <span data-ttu-id="3c94e-128">Содержит описание интереса.</span><span class="sxs-lookup"><span data-stu-id="3c94e-128">Contains a description of the interest.</span></span>                                              |
|<span data-ttu-id="3c94e-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3c94e-129">displayName</span></span>   |<span data-ttu-id="3c94e-130">Строка</span><span class="sxs-lookup"><span data-stu-id="3c94e-130">String</span></span>            | <span data-ttu-id="3c94e-131">Содержит понятное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="3c94e-131">Contains a friendly name for the interest.</span></span>                                           |
|<span data-ttu-id="3c94e-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="3c94e-132">webUrl</span></span>        |<span data-ttu-id="3c94e-133">String</span><span class="sxs-lookup"><span data-stu-id="3c94e-133">String</span></span>            | <span data-ttu-id="3c94e-134">Содержит ссылку на веб-страницу или ресурс, представляющие интерес.</span><span class="sxs-lookup"><span data-stu-id="3c94e-134">Contains a link to a webpage or resource about the interest.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="3c94e-135">Связи</span><span class="sxs-lookup"><span data-stu-id="3c94e-135">Relationships</span></span>

<span data-ttu-id="3c94e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="3c94e-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c94e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c94e-137">JSON representation</span></span>

<span data-ttu-id="3c94e-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c94e-138">The following is a JSON representation of the resource.</span></span> 

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