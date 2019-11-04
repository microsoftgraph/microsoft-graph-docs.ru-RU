---
title: Тип ресурса Итемфацет
description: Тип ресурса Итемфацет
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: bb89037b3d5b88e57ec12b2b02a5e2ed37cb2601
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939329"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="503a8-103">Тип ресурса Итемфацет</span><span class="sxs-lookup"><span data-stu-id="503a8-103">itemFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="503a8-104">Представляет абстрактный базовый тип, от которого наследуются все типы ресурсов в наборе EntitySet [профиля](profile.md) .</span><span class="sxs-lookup"><span data-stu-id="503a8-104">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="503a8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="503a8-105">Properties</span></span>

| <span data-ttu-id="503a8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="503a8-106">Property</span></span>             | <span data-ttu-id="503a8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="503a8-107">Type</span></span>                            | <span data-ttu-id="503a8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="503a8-108">Description</span></span> |
|:---------------------|:--------------------------------|:------------|
|<span data-ttu-id="503a8-109">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="503a8-109">allowedAudiences</span></span>      |<span data-ttu-id="503a8-110">string</span><span class="sxs-lookup"><span data-stu-id="503a8-110">string</span></span>                           | <span data-ttu-id="503a8-111">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="503a8-111">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="503a8-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="503a8-112">createdBy</span></span>             |[<span data-ttu-id="503a8-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="503a8-113">identitySet</span></span>](identityset.md)    | <span data-ttu-id="503a8-114">При первоначальном создании объекта.</span><span class="sxs-lookup"><span data-stu-id="503a8-114">When the entity was originally created.</span></span>   |
|<span data-ttu-id="503a8-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="503a8-115">createdDateTime</span></span>       |<span data-ttu-id="503a8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="503a8-116">DateTimeOffset</span></span>                   |<span data-ttu-id="503a8-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="503a8-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="503a8-119">id</span><span class="sxs-lookup"><span data-stu-id="503a8-119">id</span></span>                    |<span data-ttu-id="503a8-120">String</span><span class="sxs-lookup"><span data-stu-id="503a8-120">String</span></span>                           | <span data-ttu-id="503a8-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="503a8-121">Read-only.</span></span>|
|<span data-ttu-id="503a8-122">выводов</span><span class="sxs-lookup"><span data-stu-id="503a8-122">inference</span></span>             |[<span data-ttu-id="503a8-123">инференцедата</span><span class="sxs-lookup"><span data-stu-id="503a8-123">inferenceData</span></span>](inferencedata.md)| <span data-ttu-id="503a8-124">Содержит сведения о выводе, если объект определен.</span><span class="sxs-lookup"><span data-stu-id="503a8-124">Contains inference detail if the entity is inferred.</span></span> |
|<span data-ttu-id="503a8-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="503a8-125">lastModifiedBy</span></span>        |[<span data-ttu-id="503a8-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="503a8-126">identitySet</span></span>](identityset.md)    | <span data-ttu-id="503a8-127">Идентификатор партнера или пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="503a8-127">Identifier of the partner or user who last modified the entity.</span></span> |
|<span data-ttu-id="503a8-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="503a8-128">lastModifiedDateTime</span></span>  |<span data-ttu-id="503a8-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="503a8-129">DateTimeOffset</span></span>                   |<span data-ttu-id="503a8-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="503a8-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="503a8-132">Связи</span><span class="sxs-lookup"><span data-stu-id="503a8-132">Relationships</span></span>

<span data-ttu-id="503a8-133">Нет</span><span class="sxs-lookup"><span data-stu-id="503a8-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="503a8-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="503a8-134">JSON representation</span></span>

<span data-ttu-id="503a8-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="503a8-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "allowedAudiences": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "inference": {"@odata.type": "microsoft.graph.inferenceData"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemFacet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->