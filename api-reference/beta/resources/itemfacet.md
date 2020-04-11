---
title: Тип ресурса Итемфацет
description: Тип ресурса Итемфацет
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0ae0568ff5f07eacc4ea0143f79baab55b46e83b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229411"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="34383-103">Тип ресурса Итемфацет</span><span class="sxs-lookup"><span data-stu-id="34383-103">itemFacet resource type</span></span>

<span data-ttu-id="34383-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34383-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34383-105">Представляет абстрактный базовый тип, от которого наследуются все типы ресурсов в наборе EntitySet [профиля](profile.md) .</span><span class="sxs-lookup"><span data-stu-id="34383-105">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="34383-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="34383-106">Properties</span></span>

| <span data-ttu-id="34383-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="34383-107">Property</span></span>             | <span data-ttu-id="34383-108">Тип</span><span class="sxs-lookup"><span data-stu-id="34383-108">Type</span></span>                            | <span data-ttu-id="34383-109">Описание</span><span class="sxs-lookup"><span data-stu-id="34383-109">Description</span></span>                                                                                                                                                                                    |
|:---------------------|:--------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="34383-110">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="34383-110">allowedAudiences</span></span>      |<span data-ttu-id="34383-111">string</span><span class="sxs-lookup"><span data-stu-id="34383-111">string</span></span>                           | <span data-ttu-id="34383-112">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="34383-112">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>                                                   |
|<span data-ttu-id="34383-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="34383-113">createdBy</span></span>             |[<span data-ttu-id="34383-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="34383-114">identitySet</span></span>](identityset.md)    | <span data-ttu-id="34383-115">При первоначальном создании объекта.</span><span class="sxs-lookup"><span data-stu-id="34383-115">When the entity was originally created.</span></span>                                                                                                                                                        |
|<span data-ttu-id="34383-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34383-116">createdDateTime</span></span>       |<span data-ttu-id="34383-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34383-117">DateTimeOffset</span></span>                   |<span data-ttu-id="34383-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="34383-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="34383-120">id</span><span class="sxs-lookup"><span data-stu-id="34383-120">id</span></span>                    |<span data-ttu-id="34383-121">String</span><span class="sxs-lookup"><span data-stu-id="34383-121">String</span></span>                           | <span data-ttu-id="34383-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34383-122">Read-only.</span></span>                                                                                                                                                                                     |
|<span data-ttu-id="34383-123">выводов</span><span class="sxs-lookup"><span data-stu-id="34383-123">inference</span></span>             |[<span data-ttu-id="34383-124">инференцедата</span><span class="sxs-lookup"><span data-stu-id="34383-124">inferenceData</span></span>](inferencedata.md)| <span data-ttu-id="34383-125">Содержит сведения о выводе, если объект определен.</span><span class="sxs-lookup"><span data-stu-id="34383-125">Contains inference detail if the entity is inferred.</span></span>                                                                                                                                           |
|<span data-ttu-id="34383-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="34383-126">lastModifiedBy</span></span>        |[<span data-ttu-id="34383-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="34383-127">identitySet</span></span>](identityset.md)    | <span data-ttu-id="34383-128">Идентификатор партнера или пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="34383-128">Identifier of the partner or user who last modified the entity.</span></span>                                                                                                                                |
|<span data-ttu-id="34383-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34383-129">lastModifiedDateTime</span></span>  |<span data-ttu-id="34383-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34383-130">DateTimeOffset</span></span>                   |<span data-ttu-id="34383-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="34383-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="34383-133">Связи</span><span class="sxs-lookup"><span data-stu-id="34383-133">Relationships</span></span>

<span data-ttu-id="34383-134">Нет</span><span class="sxs-lookup"><span data-stu-id="34383-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34383-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34383-135">JSON representation</span></span>

<span data-ttu-id="34383-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34383-136">The following is a JSON representation of the resource.</span></span>

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