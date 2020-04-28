---
title: Тип ресурса Чанжетраккедентити
description: Представляет сущность для отслеживания изменений, внесенных в любой поддерживаемый ресурс смен
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e488fec2119f4ebf1baf5f29f62c58e7fda2789f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507756"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="9c2a9-103">Тип ресурса Чанжетраккедентити</span><span class="sxs-lookup"><span data-stu-id="9c2a9-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="9c2a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c2a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c2a9-105">Представляет сущность для отслеживания изменений, внесенных в любое поддерживаемое [Расписание](schedule.md) и связанный ресурс.</span><span class="sxs-lookup"><span data-stu-id="9c2a9-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9c2a9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c2a9-106">Properties</span></span>

| <span data-ttu-id="9c2a9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c2a9-107">Property</span></span>     | <span data-ttu-id="9c2a9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9c2a9-108">Type</span></span>        | <span data-ttu-id="9c2a9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9c2a9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9c2a9-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c2a9-110">createdDateTime</span></span>|<span data-ttu-id="9c2a9-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c2a9-111">DateTimeOffset</span></span>|<span data-ttu-id="9c2a9-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9c2a9-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9c2a9-114">id</span><span class="sxs-lookup"><span data-stu-id="9c2a9-114">id</span></span>|<span data-ttu-id="9c2a9-115">String</span><span class="sxs-lookup"><span data-stu-id="9c2a9-115">String</span></span>| <span data-ttu-id="9c2a9-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c2a9-116">Read-only.</span></span>|
|<span data-ttu-id="9c2a9-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9c2a9-117">lastModifiedBy</span></span>|[<span data-ttu-id="9c2a9-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="9c2a9-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="9c2a9-119">Идентификатор пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="9c2a9-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="9c2a9-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c2a9-120">lastModifiedDateTime</span></span>|<span data-ttu-id="9c2a9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c2a9-121">DateTimeOffset</span></span>|<span data-ttu-id="9c2a9-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9c2a9-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c2a9-124">Связи</span><span class="sxs-lookup"><span data-stu-id="9c2a9-124">Relationships</span></span>

<span data-ttu-id="9c2a9-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c2a9-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c2a9-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9c2a9-126">JSON representation</span></span>

<span data-ttu-id="9c2a9-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c2a9-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "changeTrackedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
