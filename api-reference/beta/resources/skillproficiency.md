---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6662ab205e390ae72d283d5015aa346c4b6fc2b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520508"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="fe018-103">Тип ресурса СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="fe018-103">skillProficiency resource type</span></span>

<span data-ttu-id="fe018-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fe018-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe018-105">Представляет подробные сведения о навыках, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="fe018-105">Represents detailed information about skills associated with a user in various services.</span></span>

<span data-ttu-id="fe018-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fe018-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fe018-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fe018-107">Methods</span></span>
 
| <span data-ttu-id="fe018-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fe018-108">Method</span></span>                                                 | <span data-ttu-id="fe018-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe018-109">Return Type</span></span>                             | <span data-ttu-id="fe018-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe018-110">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="fe018-111">Получение СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="fe018-111">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="fe018-112">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="fe018-112">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="fe018-113">Чтение свойств и связей объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="fe018-113">Read the properties and relationships of a **skillProficiency** object.</span></span> |
| [<span data-ttu-id="fe018-114">Обновление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="fe018-114">Update skillProficiency</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="fe018-115">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="fe018-115">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="fe018-116">Обновление объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="fe018-116">Update a **skillProficiency** object.</span></span>                               |
| [<span data-ttu-id="fe018-117">Удаление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="fe018-117">Delete skillProficiency</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="fe018-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fe018-118">None</span></span>                                    | <span data-ttu-id="fe018-119">Удаление объекта **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="fe018-119">Delete a **skillProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="fe018-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe018-120">Properties</span></span>

| <span data-ttu-id="fe018-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe018-121">Property</span></span>     | <span data-ttu-id="fe018-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fe018-122">Type</span></span>             | <span data-ttu-id="fe018-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fe018-123">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="fe018-124">categories</span><span class="sxs-lookup"><span data-stu-id="fe018-124">categories</span></span>    |<span data-ttu-id="fe018-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fe018-125">String collection</span></span> | <span data-ttu-id="fe018-126">Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный).</span><span class="sxs-lookup"><span data-stu-id="fe018-126">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span>                                       |
|<span data-ttu-id="fe018-127">displayName</span><span class="sxs-lookup"><span data-stu-id="fe018-127">displayName</span></span>   |<span data-ttu-id="fe018-128">Строка</span><span class="sxs-lookup"><span data-stu-id="fe018-128">String</span></span>            | <span data-ttu-id="fe018-129">Содержит понятное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="fe018-129">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="fe018-130">навыки</span><span class="sxs-lookup"><span data-stu-id="fe018-130">proficiency</span></span>   |<span data-ttu-id="fe018-131">строка</span><span class="sxs-lookup"><span data-stu-id="fe018-131">string</span></span>            | <span data-ttu-id="fe018-132">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fe018-132">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fe018-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="fe018-133">webUrl</span></span>        |<span data-ttu-id="fe018-134">String</span><span class="sxs-lookup"><span data-stu-id="fe018-134">String</span></span>            | <span data-ttu-id="fe018-135">Содержит ссылку на источник информации о навыке.</span><span class="sxs-lookup"><span data-stu-id="fe018-135">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="fe018-136">Связи</span><span class="sxs-lookup"><span data-stu-id="fe018-136">Relationships</span></span>

<span data-ttu-id="fe018-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fe018-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe018-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe018-138">JSON representation</span></span>

<span data-ttu-id="fe018-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe018-139">The following is a JSON representation of the resource.</span></span>

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
