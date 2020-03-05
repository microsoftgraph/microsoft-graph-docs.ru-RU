---
title: Тип ресурса Итемфацет
description: Тип ресурса Итемфацет
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: efd4977872dfefc5a0e5be9b10ad1fa196fa20a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523074"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="a9976-103">Тип ресурса Итемфацет</span><span class="sxs-lookup"><span data-stu-id="a9976-103">itemFacet resource type</span></span>

<span data-ttu-id="a9976-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a9976-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9976-105">Представляет абстрактный базовый тип, от которого наследуются все типы ресурсов в наборе EntitySet [профиля](profile.md) .</span><span class="sxs-lookup"><span data-stu-id="a9976-105">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="a9976-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9976-106">Properties</span></span>

| <span data-ttu-id="a9976-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9976-107">Property</span></span>             | <span data-ttu-id="a9976-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a9976-108">Type</span></span>                            | <span data-ttu-id="a9976-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a9976-109">Description</span></span> |
|:---------------------|:--------------------------------|:------------|
|<span data-ttu-id="a9976-110">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="a9976-110">allowedAudiences</span></span>      |<span data-ttu-id="a9976-111">строка</span><span class="sxs-lookup"><span data-stu-id="a9976-111">string</span></span>                           | <span data-ttu-id="a9976-112">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a9976-112">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="a9976-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="a9976-113">createdBy</span></span>             |[<span data-ttu-id="a9976-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="a9976-114">identitySet</span></span>](identityset.md)    | <span data-ttu-id="a9976-115">При первоначальном создании объекта.</span><span class="sxs-lookup"><span data-stu-id="a9976-115">When the entity was originally created.</span></span>   |
|<span data-ttu-id="a9976-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9976-116">createdDateTime</span></span>       |<span data-ttu-id="a9976-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9976-117">DateTimeOffset</span></span>                   |<span data-ttu-id="a9976-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a9976-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a9976-120">id</span><span class="sxs-lookup"><span data-stu-id="a9976-120">id</span></span>                    |<span data-ttu-id="a9976-121">String</span><span class="sxs-lookup"><span data-stu-id="a9976-121">String</span></span>                           | <span data-ttu-id="a9976-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9976-122">Read-only.</span></span>|
|<span data-ttu-id="a9976-123">выводов</span><span class="sxs-lookup"><span data-stu-id="a9976-123">inference</span></span>             |[<span data-ttu-id="a9976-124">инференцедата</span><span class="sxs-lookup"><span data-stu-id="a9976-124">inferenceData</span></span>](inferencedata.md)| <span data-ttu-id="a9976-125">Содержит сведения о выводе, если объект определен.</span><span class="sxs-lookup"><span data-stu-id="a9976-125">Contains inference detail if the entity is inferred.</span></span> |
|<span data-ttu-id="a9976-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a9976-126">lastModifiedBy</span></span>        |[<span data-ttu-id="a9976-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="a9976-127">identitySet</span></span>](identityset.md)    | <span data-ttu-id="a9976-128">Идентификатор партнера или пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="a9976-128">Identifier of the partner or user who last modified the entity.</span></span> |
|<span data-ttu-id="a9976-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9976-129">lastModifiedDateTime</span></span>  |<span data-ttu-id="a9976-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9976-130">DateTimeOffset</span></span>                   |<span data-ttu-id="a9976-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a9976-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9976-133">Связи</span><span class="sxs-lookup"><span data-stu-id="a9976-133">Relationships</span></span>

<span data-ttu-id="a9976-134">Нет</span><span class="sxs-lookup"><span data-stu-id="a9976-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9976-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9976-135">JSON representation</span></span>

<span data-ttu-id="a9976-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9976-136">The following is a JSON representation of the resource.</span></span>

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