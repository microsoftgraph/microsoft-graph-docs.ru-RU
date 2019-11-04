---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9490947aea170f2b6e94ecd8f02f59d396746e3a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938711"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="4411e-103">Тип ресурса СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="4411e-103">skillProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4411e-104">Представляет подробные сведения о навыках, связанных с самим пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="4411e-104">Represents detailed information about skills the user has associated with themselves in various services.</span></span>

<span data-ttu-id="4411e-105">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4411e-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4411e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4411e-106">Methods</span></span>
 
| <span data-ttu-id="4411e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4411e-107">Method</span></span>                                                 | <span data-ttu-id="4411e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4411e-108">Return Type</span></span>                             | <span data-ttu-id="4411e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4411e-109">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="4411e-110">Получение СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="4411e-110">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="4411e-111">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="4411e-111">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="4411e-112">Чтение свойств и связей объекта СкиллпрофиЦиенци.</span><span class="sxs-lookup"><span data-stu-id="4411e-112">Read properties and relationships of skillProficiency object.</span></span> |
| [<span data-ttu-id="4411e-113">Update</span><span class="sxs-lookup"><span data-stu-id="4411e-113">Update</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="4411e-114">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="4411e-114">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="4411e-115">Обновление объекта СкиллпрофиЦиенци.</span><span class="sxs-lookup"><span data-stu-id="4411e-115">Update skillProficiency object.</span></span>                               |
| [<span data-ttu-id="4411e-116">Delete</span><span class="sxs-lookup"><span data-stu-id="4411e-116">Delete</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="4411e-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="4411e-117">None</span></span>                                    | <span data-ttu-id="4411e-118">Удаление объекта СкиллпрофиЦиенци.</span><span class="sxs-lookup"><span data-stu-id="4411e-118">Delete skillProficiency object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="4411e-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4411e-119">Properties</span></span>

| <span data-ttu-id="4411e-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="4411e-120">Property</span></span>     | <span data-ttu-id="4411e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4411e-121">Type</span></span>             | <span data-ttu-id="4411e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4411e-122">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4411e-123">categories</span><span class="sxs-lookup"><span data-stu-id="4411e-123">categories</span></span>    |<span data-ttu-id="4411e-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4411e-124">String collection</span></span> | <span data-ttu-id="4411e-125">Содержит категории, связанные с навыком (например: личное, профессиональный, для увлечений)</span><span class="sxs-lookup"><span data-stu-id="4411e-125">Contains categories a user has associated with the skill (eg: personal, professional, hobby)</span></span>                                       |
|<span data-ttu-id="4411e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="4411e-126">displayName</span></span>   |<span data-ttu-id="4411e-127">Строка</span><span class="sxs-lookup"><span data-stu-id="4411e-127">String</span></span>            | <span data-ttu-id="4411e-128">Содержит понятное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="4411e-128">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="4411e-129">навыки</span><span class="sxs-lookup"><span data-stu-id="4411e-129">proficiency</span></span>   |<span data-ttu-id="4411e-130">string</span><span class="sxs-lookup"><span data-stu-id="4411e-130">string</span></span>            | <span data-ttu-id="4411e-131">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4411e-131">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4411e-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="4411e-132">webUrl</span></span>        |<span data-ttu-id="4411e-133">String</span><span class="sxs-lookup"><span data-stu-id="4411e-133">String</span></span>            | <span data-ttu-id="4411e-134">Содержит ссылку на источник информации о навыке.</span><span class="sxs-lookup"><span data-stu-id="4411e-134">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="4411e-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4411e-135">Relationships</span></span>

<span data-ttu-id="4411e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4411e-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4411e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4411e-137">JSON representation</span></span>

<span data-ttu-id="4411e-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4411e-138">The following is a JSON representation of the resource.</span></span>

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