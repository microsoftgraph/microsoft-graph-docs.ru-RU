---
title: тип ресурса changeTrackedEntity
description: Представляет объект для отслеживания изменений, внесенных в любой поддерживаемый ресурс Shifts.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e02c02b931558b927f29e7b08a18c5d5937f0f72
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720216"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="63e91-103">тип ресурса changeTrackedEntity</span><span class="sxs-lookup"><span data-stu-id="63e91-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="63e91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63e91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63e91-105">Представляет объект для отслеживания изменений, внесенных в любое поддерживаемый [график](schedule.md) и связанный ресурс.</span><span class="sxs-lookup"><span data-stu-id="63e91-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="63e91-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="63e91-106">Properties</span></span>

| <span data-ttu-id="63e91-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="63e91-107">Property</span></span>     | <span data-ttu-id="63e91-108">Тип</span><span class="sxs-lookup"><span data-stu-id="63e91-108">Type</span></span>        | <span data-ttu-id="63e91-109">Описание</span><span class="sxs-lookup"><span data-stu-id="63e91-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63e91-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63e91-110">createdDateTime</span></span>|<span data-ttu-id="63e91-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63e91-111">DateTimeOffset</span></span>|<span data-ttu-id="63e91-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="63e91-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="63e91-113">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="63e91-113">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="63e91-114">id</span><span class="sxs-lookup"><span data-stu-id="63e91-114">id</span></span>|<span data-ttu-id="63e91-115">String</span><span class="sxs-lookup"><span data-stu-id="63e91-115">String</span></span>| <span data-ttu-id="63e91-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="63e91-116">Read-only.</span></span>|
|<span data-ttu-id="63e91-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="63e91-117">lastModifiedBy</span></span>|[<span data-ttu-id="63e91-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="63e91-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="63e91-119">Удостоверение человека, который в последний раз изменил объект.</span><span class="sxs-lookup"><span data-stu-id="63e91-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="63e91-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63e91-120">lastModifiedDateTime</span></span>|<span data-ttu-id="63e91-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63e91-121">DateTimeOffset</span></span>|<span data-ttu-id="63e91-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="63e91-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="63e91-123">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="63e91-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="63e91-124">Связи</span><span class="sxs-lookup"><span data-stu-id="63e91-124">Relationships</span></span>

<span data-ttu-id="63e91-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="63e91-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63e91-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="63e91-126">JSON representation</span></span>

<span data-ttu-id="63e91-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63e91-127">The following is a JSON representation of the resource.</span></span>

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


