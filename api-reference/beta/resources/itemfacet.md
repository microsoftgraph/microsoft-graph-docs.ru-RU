---
title: Тип ресурса Итемфацет
description: Тип ресурса Итемфацет
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b32baed9dd6bad45f37b7be24b67308e0624b42c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809399"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="1a8c6-103">Тип ресурса Итемфацет</span><span class="sxs-lookup"><span data-stu-id="1a8c6-103">itemFacet resource type</span></span>

<span data-ttu-id="1a8c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a8c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a8c6-105">Представляет абстрактный базовый тип, от которого наследуются все типы ресурсов в наборе EntitySet [профиля](profile.md) .</span><span class="sxs-lookup"><span data-stu-id="1a8c6-105">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="1a8c6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a8c6-106">Properties</span></span>
|<span data-ttu-id="1a8c6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a8c6-107">Property</span></span>|<span data-ttu-id="1a8c6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1a8c6-108">Type</span></span>|<span data-ttu-id="1a8c6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1a8c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a8c6-110">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="1a8c6-110">allowedAudiences</span></span>|<span data-ttu-id="1a8c6-111">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="1a8c6-111">allowedAudiences</span></span>|<span data-ttu-id="1a8c6-112">Аудитории, которые могут просматривать значения, содержащиеся в связанном объекте.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-112">The audiences that are able to see the values contained within the associated entity.</span></span> <span data-ttu-id="1a8c6-113">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-113">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1a8c6-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="1a8c6-114">createdBy</span></span>|[<span data-ttu-id="1a8c6-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="1a8c6-115">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="1a8c6-116">Предоставляет идентификатор пользователя и/или приложения, создавшего сущность.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-116">Provides the identifier of the user and/or application that created the entity.</span></span>|
|<span data-ttu-id="1a8c6-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a8c6-117">createdDateTime</span></span>|<span data-ttu-id="1a8c6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a8c6-118">DateTimeOffset</span></span>|<span data-ttu-id="1a8c6-119">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-119">Provides the dateTimeOffset for when the entity was created.</span></span>|
|<span data-ttu-id="1a8c6-120">id</span><span class="sxs-lookup"><span data-stu-id="1a8c6-120">id</span></span>|<span data-ttu-id="1a8c6-121">String</span><span class="sxs-lookup"><span data-stu-id="1a8c6-121">String</span></span>|<span data-ttu-id="1a8c6-122">Идентификатор, используемый для индивидуальной адресации объекта.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-122">Identifier used for individually addressing an entity.</span></span> <span data-ttu-id="1a8c6-123">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="1a8c6-123">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="1a8c6-124">выводов</span><span class="sxs-lookup"><span data-stu-id="1a8c6-124">inference</span></span>|[<span data-ttu-id="1a8c6-125">инференцедата</span><span class="sxs-lookup"><span data-stu-id="1a8c6-125">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1a8c6-126">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-126">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span>|
|<span data-ttu-id="1a8c6-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1a8c6-127">lastModifiedBy</span></span>|[<span data-ttu-id="1a8c6-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="1a8c6-128">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="1a8c6-129">Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-129">Provides the identifier of the user and/or application that last modified the entity.</span></span>|
|<span data-ttu-id="1a8c6-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a8c6-130">lastModifiedDateTime</span></span>|<span data-ttu-id="1a8c6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a8c6-131">DateTimeOffset</span></span>|<span data-ttu-id="1a8c6-132">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-132">Provides the dateTimeOffset for when the entity was created.</span></span>|
|<span data-ttu-id="1a8c6-133">source</span><span class="sxs-lookup"><span data-stu-id="1a8c6-133">source</span></span>|[<span data-ttu-id="1a8c6-134">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="1a8c6-134">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="1a8c6-135">Источник значений в сущности при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-135">Where the values within an entity originated if synced from another service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a8c6-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="1a8c6-136">Relationships</span></span>
<span data-ttu-id="1a8c6-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a8c6-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1a8c6-138">JSON representation</span></span>
<span data-ttu-id="1a8c6-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a8c6-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemFacet",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  }
}
```

