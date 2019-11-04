---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0bb63903b5a3eb0eeed8683463b9927537180f53
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950425"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="f1f90-103">Тип ресурса СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1f90-103">skillProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f90-104">Представляет подробные сведения о навыках, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="f1f90-104">Represents detailed information about skills associated with a user in various services.</span></span>

<span data-ttu-id="f1f90-105">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f1f90-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f1f90-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f1f90-106">Methods</span></span>
 
| <span data-ttu-id="f1f90-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f1f90-107">Method</span></span>                                                 | <span data-ttu-id="f1f90-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f1f90-108">Return Type</span></span>                             | <span data-ttu-id="f1f90-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f1f90-109">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="f1f90-110">Получение СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1f90-110">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="f1f90-111">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1f90-111">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="f1f90-112">Чтение свойств и связей объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="f1f90-112">Read the properties and relationships of a **skillProficiency** object.</span></span> |
| [<span data-ttu-id="f1f90-113">Обновление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1f90-113">Update skillProficiency</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="f1f90-114">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1f90-114">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="f1f90-115">Обновление объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="f1f90-115">Update a **skillProficiency** object.</span></span>                               |
| [<span data-ttu-id="f1f90-116">Удаление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1f90-116">Delete skillProficiency</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="f1f90-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1f90-117">None</span></span>                                    | <span data-ttu-id="f1f90-118">Удаление объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="f1f90-118">Delete a **skillProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="f1f90-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1f90-119">Properties</span></span>

| <span data-ttu-id="f1f90-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1f90-120">Property</span></span>     | <span data-ttu-id="f1f90-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f1f90-121">Type</span></span>             | <span data-ttu-id="f1f90-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f1f90-122">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f1f90-123">categories</span><span class="sxs-lookup"><span data-stu-id="f1f90-123">categories</span></span>    |<span data-ttu-id="f1f90-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1f90-124">String collection</span></span> | <span data-ttu-id="f1f90-125">Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный).</span><span class="sxs-lookup"><span data-stu-id="f1f90-125">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span>                                       |
|<span data-ttu-id="f1f90-126">displayName</span><span class="sxs-lookup"><span data-stu-id="f1f90-126">displayName</span></span>   |<span data-ttu-id="f1f90-127">Строка</span><span class="sxs-lookup"><span data-stu-id="f1f90-127">String</span></span>            | <span data-ttu-id="f1f90-128">Содержит понятное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="f1f90-128">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="f1f90-129">навыки</span><span class="sxs-lookup"><span data-stu-id="f1f90-129">proficiency</span></span>   |<span data-ttu-id="f1f90-130">string</span><span class="sxs-lookup"><span data-stu-id="f1f90-130">string</span></span>            | <span data-ttu-id="f1f90-131">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f1f90-131">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f1f90-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="f1f90-132">webUrl</span></span>        |<span data-ttu-id="f1f90-133">String</span><span class="sxs-lookup"><span data-stu-id="f1f90-133">String</span></span>            | <span data-ttu-id="f1f90-134">Содержит ссылку на источник информации о навыке.</span><span class="sxs-lookup"><span data-stu-id="f1f90-134">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="f1f90-135">Связи</span><span class="sxs-lookup"><span data-stu-id="f1f90-135">Relationships</span></span>

<span data-ttu-id="f1f90-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f1f90-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1f90-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f1f90-137">JSON representation</span></span>

<span data-ttu-id="f1f90-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1f90-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "displayName": "String",
  "proficiency": "string",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "skillProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
