---
title: Тип ресурса ЛангуажепрофиЦиенци
description: Тип ресурса ЛангуажепрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 3a022d9c255bbfee03ef7f1fec891bc0fa757480
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950460"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="6abd6-103">Тип ресурса ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="6abd6-103">languageProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6abd6-104">Представляет подробные сведения о языках, добавленных пользователем в свой [профиль](profile.md).</span><span class="sxs-lookup"><span data-stu-id="6abd6-104">Represents detailed information about languages that a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="6abd6-105">Наследуется от [итемфацет](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="6abd6-105">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6abd6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6abd6-106">Methods</span></span>

| <span data-ttu-id="6abd6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6abd6-107">Method</span></span>                                                       | <span data-ttu-id="6abd6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6abd6-108">Return Type</span></span>                                   | <span data-ttu-id="6abd6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6abd6-109">Description</span></span>                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="6abd6-110">Получение ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="6abd6-110">Get languageProficiency</span></span>](../api/languageproficiency-get.md) | [<span data-ttu-id="6abd6-111">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="6abd6-111">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="6abd6-112">Чтение свойств и связей объекта **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="6abd6-112">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="6abd6-113">Обновление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="6abd6-113">Update languageProficiency</span></span>](../api/languageproficiency-update.md)               | [<span data-ttu-id="6abd6-114">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="6abd6-114">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="6abd6-115">Обновление объекта **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="6abd6-115">Update a **languageProficiency** object.</span></span>                               |
| [<span data-ttu-id="6abd6-116">Удаление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="6abd6-116">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)               | <span data-ttu-id="6abd6-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="6abd6-117">None</span></span>                                          | <span data-ttu-id="6abd6-118">Удаление объекта **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="6abd6-118">Delete a **languageProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="6abd6-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="6abd6-119">Properties</span></span>

| <span data-ttu-id="6abd6-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="6abd6-120">Property</span></span>     | <span data-ttu-id="6abd6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6abd6-121">Type</span></span>        | <span data-ttu-id="6abd6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6abd6-122">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6abd6-123">displayName</span><span class="sxs-lookup"><span data-stu-id="6abd6-123">displayName</span></span>   |<span data-ttu-id="6abd6-124">String</span><span class="sxs-lookup"><span data-stu-id="6abd6-124">String</span></span>       | <span data-ttu-id="6abd6-125">Содержит имя языка в длинном формате.</span><span class="sxs-lookup"><span data-stu-id="6abd6-125">Contains the long-form name for the language.</span></span>                                                                                                   |
|<span data-ttu-id="6abd6-126">навыки</span><span class="sxs-lookup"><span data-stu-id="6abd6-126">proficiency</span></span>   |<span data-ttu-id="6abd6-127">string</span><span class="sxs-lookup"><span data-stu-id="6abd6-127">string</span></span>       | <span data-ttu-id="6abd6-128">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6abd6-128">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6abd6-129">tag</span><span class="sxs-lookup"><span data-stu-id="6abd6-129">tag</span></span>           |<span data-ttu-id="6abd6-130">String</span><span class="sxs-lookup"><span data-stu-id="6abd6-130">String</span></span>       | <span data-ttu-id="6abd6-131">Содержит четырехзначный BCP47 Name для языка (EN-US, No-NetBIOS, en-AU).</span><span class="sxs-lookup"><span data-stu-id="6abd6-131">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                                  |

## <a name="relationships"></a><span data-ttu-id="6abd6-132">Связи</span><span class="sxs-lookup"><span data-stu-id="6abd6-132">Relationships</span></span>

<span data-ttu-id="6abd6-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6abd6-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6abd6-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6abd6-134">JSON representation</span></span>

<span data-ttu-id="6abd6-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6abd6-135">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "proficiency": "string",
  "tag": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "languageProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
