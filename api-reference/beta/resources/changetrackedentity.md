---
title: Тип ресурса Чанжетраккедентити
description: Представляет сущность для отслеживания изменений, внесенных в любой поддерживаемый ресурс смен
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c420274f6ff8e0521f9fd5baca193e95334f3de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042697"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="5b21c-103">Тип ресурса Чанжетраккедентити</span><span class="sxs-lookup"><span data-stu-id="5b21c-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="5b21c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b21c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b21c-105">Представляет сущность для отслеживания изменений, внесенных в любое поддерживаемое [Расписание](schedule.md) и связанный ресурс.</span><span class="sxs-lookup"><span data-stu-id="5b21c-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="5b21c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b21c-106">Properties</span></span>

| <span data-ttu-id="5b21c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b21c-107">Property</span></span>     | <span data-ttu-id="5b21c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5b21c-108">Type</span></span>        | <span data-ttu-id="5b21c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5b21c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b21c-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b21c-110">createdDateTime</span></span>|<span data-ttu-id="5b21c-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b21c-111">DateTimeOffset</span></span>|<span data-ttu-id="5b21c-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5b21c-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5b21c-114">id</span><span class="sxs-lookup"><span data-stu-id="5b21c-114">id</span></span>|<span data-ttu-id="5b21c-115">String</span><span class="sxs-lookup"><span data-stu-id="5b21c-115">String</span></span>| <span data-ttu-id="5b21c-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b21c-116">Read-only.</span></span>|
|<span data-ttu-id="5b21c-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5b21c-117">lastModifiedBy</span></span>|[<span data-ttu-id="5b21c-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="5b21c-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="5b21c-119">Идентификатор пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="5b21c-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="5b21c-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b21c-120">lastModifiedDateTime</span></span>|<span data-ttu-id="5b21c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b21c-121">DateTimeOffset</span></span>|<span data-ttu-id="5b21c-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5b21c-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b21c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="5b21c-124">Relationships</span></span>

<span data-ttu-id="5b21c-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5b21c-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b21c-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5b21c-126">JSON representation</span></span>

<span data-ttu-id="5b21c-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b21c-127">The following is a JSON representation of the resource.</span></span>

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


