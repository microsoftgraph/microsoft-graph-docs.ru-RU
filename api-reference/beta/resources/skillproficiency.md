---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7c8b5a3711c7abdbbdd8ddba8f7a36c85978718b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228875"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="a2d75-103">Тип ресурса СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="a2d75-103">skillProficiency resource type</span></span>

<span data-ttu-id="a2d75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2d75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2d75-105">Представляет подробные сведения о навыках, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="a2d75-105">Represents detailed information about skills associated with a user in various services.</span></span>

<span data-ttu-id="a2d75-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a2d75-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a2d75-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a2d75-107">Methods</span></span>
 
| <span data-ttu-id="a2d75-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a2d75-108">Method</span></span>                                                         | <span data-ttu-id="a2d75-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a2d75-109">Return Type</span></span>                             | <span data-ttu-id="a2d75-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2d75-110">Description</span></span>                                                             |
|:---------------------------------------------------------------|:----------------------------------------|:------------------------------------------------------------------------|
| [<span data-ttu-id="a2d75-111">Получение СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="a2d75-111">Get skillProficiency</span></span>](../api/skillproficiency-get.md)         | [<span data-ttu-id="a2d75-112">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="a2d75-112">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="a2d75-113">Чтение свойств и связей объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="a2d75-113">Read the properties and relationships of a **skillProficiency** object.</span></span> |
| [<span data-ttu-id="a2d75-114">Обновление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="a2d75-114">Update skillProficiency</span></span>](../api/skillproficiency-update.md)   | [<span data-ttu-id="a2d75-115">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="a2d75-115">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="a2d75-116">Обновление объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="a2d75-116">Update a **skillProficiency** object.</span></span>                                   |
| [<span data-ttu-id="a2d75-117">Удаление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="a2d75-117">Delete skillProficiency</span></span>](../api/skillproficiency-delete.md)   | <span data-ttu-id="a2d75-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a2d75-118">None</span></span>                                    | <span data-ttu-id="a2d75-119">Удаление объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="a2d75-119">Delete a **skillProficiency** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="a2d75-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2d75-120">Properties</span></span>

| <span data-ttu-id="a2d75-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2d75-121">Property</span></span>     | <span data-ttu-id="a2d75-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a2d75-122">Type</span></span>             | <span data-ttu-id="a2d75-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a2d75-123">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="a2d75-124">categories</span><span class="sxs-lookup"><span data-stu-id="a2d75-124">categories</span></span>    |<span data-ttu-id="a2d75-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a2d75-125">String collection</span></span> | <span data-ttu-id="a2d75-126">Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный).</span><span class="sxs-lookup"><span data-stu-id="a2d75-126">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span>                             |
|<span data-ttu-id="a2d75-127">displayName</span><span class="sxs-lookup"><span data-stu-id="a2d75-127">displayName</span></span>   |<span data-ttu-id="a2d75-128">Строка</span><span class="sxs-lookup"><span data-stu-id="a2d75-128">String</span></span>            | <span data-ttu-id="a2d75-129">Содержит понятное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="a2d75-129">Contains a friendly name for the skill.</span></span>                                                                                            |
|<span data-ttu-id="a2d75-130">навыки</span><span class="sxs-lookup"><span data-stu-id="a2d75-130">proficiency</span></span>   |<span data-ttu-id="a2d75-131">string</span><span class="sxs-lookup"><span data-stu-id="a2d75-131">string</span></span>            | <span data-ttu-id="a2d75-132">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a2d75-132">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a2d75-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="a2d75-133">webUrl</span></span>        |<span data-ttu-id="a2d75-134">String</span><span class="sxs-lookup"><span data-stu-id="a2d75-134">String</span></span>            | <span data-ttu-id="a2d75-135">Содержит ссылку на источник информации о навыке.</span><span class="sxs-lookup"><span data-stu-id="a2d75-135">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="a2d75-136">Связи</span><span class="sxs-lookup"><span data-stu-id="a2d75-136">Relationships</span></span>

<span data-ttu-id="a2d75-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a2d75-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2d75-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a2d75-138">JSON representation</span></span>

<span data-ttu-id="a2d75-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2d75-139">The following is a JSON representation of the resource.</span></span>

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
